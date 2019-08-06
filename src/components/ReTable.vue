<template>
    <div>
      <table class="table table-bordered table-dark">
        <thead>
          <th v-for="(column, key) in tableData[1]" :key="key">
            {{ key }}
          </th>
        </thead>
        <tbody>
          <tr v-for="(column) in tableData" :key="column.id">
            <td v-for="row in column" :key="row">
              {{ row }}
            </td>
          </tr>
        </tbody>
      </table>
    </div>
</template>

<script>
export default {
  name: 'ReTable',
  props: [
    'tableData',
  ],
  data() {
    return {
    };
  },
  computed: {
    columns() {
      return Object.keys(this.tableData[1]).length;
    },
  },
};
</script>

<style>
@import "https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css";

</style>
