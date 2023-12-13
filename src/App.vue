<template>
  <div class="container">
    <h2>App Components</h2>
    <input type="text" placeholder="Say something.." v-model="msg">
    <Products :greetings="msg"/> <!--assigning a variable to a property, (msg is a variable)-->
    <Products greetings="Class1"/> <!--child component-->
  </div>
</template>

<script>
import Products from './components/Products.vue'

export default {
  name: 'App',
  data() {
    return {
      msg: ''
    
  }
  },
  components: {
    Products
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color:white;
  margin-top: 60px;
}

</style>
