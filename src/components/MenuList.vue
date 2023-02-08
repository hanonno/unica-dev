<template>
  <ol>
    <MenuItem v-for="(item, index) in menuItems" v-bind:text="item.text" />
  </ol>
</template>

<script>
import MenuItem from './MenuItem.vue';

export default {
  name: 'MenuList',
  components: {
    MenuItem,
  },
  props: {
    text: String,
    menuItems: [],
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ol {
  padding: 0 0 0 16px;
}

li {
  color: #42b983;
  list-style-type: none;
}
</style>
