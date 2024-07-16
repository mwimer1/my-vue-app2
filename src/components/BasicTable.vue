<template>
  <table>
    <thead>
      <tr>
        <th>Name</th>
        <th>Age</th>
        <th>Address</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="item in data" :key="item.id">
        <td>{{ item.name }}</td>
        <td>{{ item.age }}</td>
        <td>{{ item.address }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>
import { defineComponent, ref } from 'vue';

export default defineComponent({
  name: 'BasicTable',
  setup() {
    const data = ref([
      { id: 1, name: 'John Brown', age: 32, address: 'New York No. 1 Lake Park' },
      { id: 2, name: 'Jim Green', age: 42, address: 'London No. 1 Lake Park' },
      { id: 3, name: 'Joe Black', age: 32, address: 'Sidney No. 1 Lake Park' },
    ]);

    return {
      data,
    };
  },
});
</script>

<style scoped>
table {
  width: 100%;
  border-collapse: collapse;
}

th, td {
  border: 1px solid #ddd;
  padding: 8px;
}

th {
  background-color: #f2f2f2;
}
</style>
