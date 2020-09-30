<template>
  <div id="app">
    <blogheader msg="Welcome to Your Vue.js App"/>
    <contents />
    <foot/>
  </div>
</template>

<script>
import blogheader from './components/header.vue'
import contents from './components/content.vue'
import foot from './components/footer.vue'

export default {
  name: 'App',
  components: {
   blogheader,
   contents,
   foot
  }
}
</script>

<style>

</style>
