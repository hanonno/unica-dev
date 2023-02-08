<template>
  <div class="button round">{{ text }}</div>
</template>

<script>
export default {
  name: 'ButtonRound',
  props: {
    text: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div.button {
  display: inline-block;
  width: 32px;
  height: 32px;
  background-color: #dee1e6;
}
</style>
