<template>
  <div id="app">
    <BasicTable />
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import BasicTable from './components/BasicTable.vue';

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
