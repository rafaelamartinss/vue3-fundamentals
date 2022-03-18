<template>
  <div id="app">
    <AppPlan v-for="plan in plans" :name="plan" />
  </div>
</template>

<script>
import AppPlan from './components/AppPlan.vue';

export default {
  name: 'App',
  components: {
    AppPlan,
  },
  data() {
    return {
      plans: ['Coffee', 'Frapuccino', 'Black Coffee'],
    };
  },
};
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
