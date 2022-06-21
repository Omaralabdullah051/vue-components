<template>
  <!-- <Greet name="Bruce" hero-name="Batman"/>
  <Greet name="Clark" hero-name="Superman"/>
  <Greet name="Michell" hero-name="Ironman"/>
  <Greet :name="name" :hero-name="heroName"/> -->

  <Article id="my-article" title="Article Title" :likes="50" :isPublished="true" :object="{name:'batman'}"/>
</template>

<script>
// import Greet from './components/Greet.vue';
import Article from "./components/Article.vue";

export default {
  name: 'App',
  components: {
    // Greet,
    Article,
  },
  data(){
    return {
      name: 'Wrayne',
      heroName: 'Spiderman'
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
