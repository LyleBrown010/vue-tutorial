<template>
  <div class="home">
    <FormComp/>
    <!-- <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    

  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import FormComp from '@/components/Form-Comp.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld, FormComp
  }
}
</script>
