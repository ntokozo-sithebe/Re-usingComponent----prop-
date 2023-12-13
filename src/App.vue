<template>
  <div>
    <div class="container">
    <h2>App Component</h2>
    <input type="text" placeholder="Say Something" v-model="msg">
    <Products :greeting="msg" />
    <!-- <Products greeting="Class 1"/> -->
  </div>
  </div>
  
</template>

<script>
import Products from './components/Products.vue';
export default {
  name: 'App',
  data(){
    return{
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
  color: #2c3e50;
  margin-top: 60px;
}
.container{
  background-color:  rgba(68, 68, 208, 0.44); ;
}
</style>
