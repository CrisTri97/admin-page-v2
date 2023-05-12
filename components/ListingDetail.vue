<template>
  <div class="center content-inputs container">
    <vs-input
      v-model="value"
      class="input-item-detail"
      placeholder="The wayuu The Dreamcatcher"
    />
  </div>
</template>
<script>
export default {
  data: () => ({
    value: '',
  }),
}
</script>

<style lang="scss">
.container {
  width: 100%;
  .input-item-detail input {
    width: 100%;
  }
}
</style>
