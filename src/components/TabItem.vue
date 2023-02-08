<template>
  <div class="tab-item">
    <a href="#">{{ text }}haha</a>
  </div>
</template>

<script>
export default {
  name: 'TabItem',
  props: {
    text: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.tab-item {
  padding: 5px 16px;

  background-color: #dee1e6;
}
</style>
