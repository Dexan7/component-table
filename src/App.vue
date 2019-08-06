<template>
  <div id="app">
    <ReTable :tableData="tableData"></ReTable>
  </div>
</template>


<script>
import ReTable from './components/ReTable.vue';

export default {
  name: 'app',
  components: {
    ReTable,
  },
  data() {
    return {
      tableData: [{
        date: '2016-05-03',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
        test: 'sdfgsdf',
      }, {
        date: '2016-05-02',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
        test: 'sdfgsdf',
      }, {
        date: '2016-05-04',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
        test: 'sdfgsdf',
      }, {
        date: '2016-05-01',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
        test: 'sdfgsdf',
      }, {
        date: '2016-05-01',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
        test: 'sdfgsdf',
      }],
    };
  },
};
</script>

<style>

</style>
