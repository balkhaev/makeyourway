<style>
  .card-container {
    margin-top: 20px;
  }
</style>

<template>
  <div class="card-container">
    <a-row :gutter="16">
      <a-col class="gutter-row" :span="4" v-for="list in lists" :key="list">
        <list :title="list">
          <card></card>
        </list>
      </a-col>
    </a-row>
  </div>
</template>

<script>
  import Card from '../components/Card';
  import List from '../components/List';

  export default {
    name: 'home',
    components: {
      Card,
      List,
    },
    data: () => ({
      lists: ['Backlog', 'Tasks', 'WIP', 'Review', 'Tests', 'Prod'],
    })
  }
</script>
