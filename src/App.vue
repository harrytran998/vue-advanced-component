<template>
  <div id="app">
    <!-- <date-picker
      v-model="date"
      format="DD-MM-YYYY"
      :options="{ firstDay: 2 }"
    /> -->
    <test-scoped-slot></test-scoped-slot>
  </div>
</template>

<script>
// import DatePicker from './components/common/DatePicker.vue'
import TestScopedSlot from './components/Slot/TestSlot'
export default {
  name: 'App',
  components: {
    TestScopedSlot,
  },
  data: () => ({
    date: '10-10-2020',
  }),
}
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
