<template>
  <navbar/>
  <mainContent/>
</template>

<script>
import navbar from './navigation.vue'
import mainContent from './welcomeContent.vue'
export default {
  name: "mainPage",
  components:{
    navbar,
    mainContent,
  }
}
</script>

<style>

</style>