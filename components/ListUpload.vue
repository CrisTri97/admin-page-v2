<template>
  <div class="center-x upload-container">
    <vs-upload  class="upload-item" action="https://jsonplaceholder.typicode.com/posts/" @on-success="successUpload" 
    />
  </div>
</template>

<script>
export default {
  name: 'ListUpload',
  methods: {
    successUpload() {
      this.$vs.notify({
        color: 'success',
        title: 'Upload Success',
        text: 'Lorem ipsum dolor sit amet, consectetur',
      })
    },
  },
}
</script>

<style lang="scss">
    .upload-container {
        width: 150px;
        height: 150px;
        display: block;
        .upload-item {
            width: 100%;
            height: 100%;
            color: bisque;
        }
    }
</style>
