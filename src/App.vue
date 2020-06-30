<template>
  <div id="app">
    <!-- <date-picker
      v-model="date"
      format="DD-MM-YYYY"
      :options="{ firstDay: 2 }"
    />-->
    <!-- <test-scoped-slot></test-scoped-slot> -->
    <parent-base-input></parent-base-input>
  </div>
</template>

<script>
// import DatePicker from './components/common/DatePicker.vue'
import ParentBaseInput from "./components/EdgeCases/ParentBaseInput";
export default {
  components: {
    ParentBaseInput
  }
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
