<template>
  <div id="app">
    <BasicTable />
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import BasicTable from './components/wwElement.vue';

export default defineComponent({
  name: 'App',
  components: {
    BasicTable,
  },
});
</script>

<style>
/* Add any custom styles here */
</style>
