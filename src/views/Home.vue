<template lang="pug">
.home
  img(alt="Vue logo" src="../assets/logo.png")
  hello-world(msg="Welcome to Your Vue.js App")
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld
  }
};
</script>

<style lang="sass">
img
  margin-bottom: 0
</style>
