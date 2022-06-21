<template>
  <button @click="showPopupMethod">Show Popup</button>
  <Popup v-show="showPopup" @close="closePopup"/>
  <h2 v-if="name">Name -{{name}}</h2>
</template>

<script>
import Popup from './components/Popup.vue';

export default {
  name: 'App',
  components: {
    Popup
  },
  data(){
    return {
       showPopup: false,
       name: '',
    }
  },
  methods: {
    showPopupMethod(){
      this.showPopup = true;
      this.name = '';
    },
    closePopup(name){
      this.showPopup = false;
      this.name = name
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
