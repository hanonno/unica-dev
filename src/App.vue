<template>
  <div id="app">
    <Navigation />
    <MenuList v-bind:menuItems="menuItems">
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import Navigation from "./components/Navigation.vue";
import MenuList from './components/MenuList.vue';

export default {
  name: 'App',
  components: {
    Navigation,
    MenuList,
  },
  data() {
    return {
      menuItems: [{ text: 'Commerce' }, { text: 'Development' }, { text: 'Risk' }, { text: 'Home' }],
    };
  },
};
</script>

<style>

body {
  margin:0; padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  margin: 0;
  padding: 0;

  background-color: #EEF0F3;
}
</style>
