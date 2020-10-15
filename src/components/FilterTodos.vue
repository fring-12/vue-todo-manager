<template>
  <div class="filter">
    <h3>Filter Todos</h3>
    <select @change="filterTodos($event)">
      <option value="200">200</option>
      <option value="100">100</option>
      <option value="50">50</option>
      <option value="20">20</option>
      <option value="5">5</option>
    </select>

  </div>
</template>

<script>
import {mapActions} from 'vuex'

  export default {
    name: "FilterTodos",
    methods: mapActions(["filterTodos"])
  }
</script>

<style scoped>
.filter{
  display: flex;
}
select{
  padding: 5px;
  margin: 20px;
  border: 1px solid #41b883;
  border-radius: 2px;
}

</style>