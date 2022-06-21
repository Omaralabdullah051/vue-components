<template>
  <h3>AppComponent {{name}}</h3>
  <ComponentC/>
</template>

<script>
import ComponentC from "./components/ComponentC.vue";

export default {
  name: 'App',
  components: {
    ComponentC
  },
  data(){
    return {
      name: 'Bruce'
    }
  },
  //When we need to provide data without prop-drilling and cannot add it to the App component.
  // provide: {
  //   username: 'Bruce'
  // }
  //or
  //When we need to provide data without prop-drilling and also can add it to the App component.
  provide(){
    return {
      username: this.name
    }
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
</style>
