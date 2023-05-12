<template>
  <div>
    <h3>Select up to 2</h3>
    <div class="text-area-container">
      <div class="center con-checkbox">
        <vs-checkbox v-model="options" val="html"> Html </vs-checkbox>
        <vs-checkbox v-model="options" val="css"> Css </vs-checkbox>
        <vs-checkbox v-model="options" val="javascript">
          Javascript
        </vs-checkbox>
        <vs-checkbox v-model="options" val="vue"> Vue </vs-checkbox>
        <vs-checkbox v-model="options" val="vuesax"> Vuesax </vs-checkbox>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TextAreaCheckBox',
  data: () => ({
    options: ['javascript', 'vue'],
  }),
}
</script>

<style lang="scss">
.text-area-container {
  width: 300px;
  height: 100px;
  overflow-y: scroll;
  padding: 10px;
  border: 1px solid rgb(184, 184, 184);
}
</style>
