<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Dynamic Layouts Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

import Index from "@/layouts/Index.vue"

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  created() {
    this.$emit("update:layout", Index)
  }
}
</script>
