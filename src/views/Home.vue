<template>
  <div class="home">
    <img alt="FridgiGo logo" src="../assets/FridgiGoLogo250.png">
    <HelloWorld msg="Welcome to the secured FridgiGo App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: "Home",
  components: {
    HelloWorld
  }
}
</script>

<style scoped>

</style>