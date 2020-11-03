<template>
  <div id="app">
    <budgetList :list='list' />
  </div>
</template>

<script>
import budgetList from '@/components/budgetList';

export default {
  name: 'App',
  components: {
    budgetList,
  },
  data: () => ({
    list: {
      1: {
        type: 'INCOME',
        value: 100,
        comment: 'Some Comment',
        id: 1,
      },
    },
  }),
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2d4761;
  margin-top: 60px;
}
</style>
