<template>
  <li>
    <a href="#">{{ text }}</a>
  </li>
</template>

<script>
export default {
  name: 'MenuItem',
  props: {
    text: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
a {
  color: #42b983;
}
</style>
