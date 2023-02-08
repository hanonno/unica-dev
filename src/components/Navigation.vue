<template>
  <div id="navigation">
    <section class="company">Nike Inc.</section>

    <section class="sections">
      <TabItem text="Overview" />
      <TabItem text="Accounts" />
      <TabItem text="Teams" />
    </section>

    <section class="buttons">
      <ButtonRound v-bind:text="Search" />
      <ButtonRound v-bind:text="Notifications" />
      <ButtonRound v-bind:text="Help" />
    </section>
  </div>
</template>

<script>
import TabItem from './TabItem.vue';
import ButtonRound from './ButtonRound.vue';

export default {
  name: 'Navigation',
  components: {
    TabItem,
    ButtonRound,
  },
  props: {
    text: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#navigation {
  display: flex;

  padding: 16px;

  justify-content: space-between;
}

section {
  display: flex;
  gap: 16px;
}

section.company {
  padding: 5px 0;
  font-weight: bold;
}
</style>
