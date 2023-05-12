<template>
  <div class="centerx">
    <div class="category-container">
      <h3>Shopper will find this item in all of these categories</h3>
      <div>
        <span class="tag-category" v-for="item in value" :key="item">
          {{ item }}
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: Array,
      required: false,
      default: () => [],
    },
  },
}
</script>

<style lang="scss">
.category-container {
  display: flex;
  width: 100%;
  flex-direction: column;
  .tag-category {
    padding: 5px;
    border-radius: 5px;
    border: 1px solid rgb(216, 215, 215);
    margin-right: 5px;
  }
}
</style>
