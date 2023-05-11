<template id="root">
 <HomeComponent/>
</template>

<script lang="ts">
import Vue from 'vue'
import Vuesax from 'vuesax'
import 'vuesax/dist/vuesax.css'
import 'boxicons/css/boxicons.min.css'


Vue.use(Vuesax, {
  rtl: false
})
export default {
    name: "index",
}
</script>

<style>
a {
  text-decoration: none;
  color: black;
}
</style>
