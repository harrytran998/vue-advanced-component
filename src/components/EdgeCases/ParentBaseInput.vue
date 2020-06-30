<template>
  <fragment>
    <h1 class="text-6xl">Hello Focus Input</h1>
    <base-input ref="userInput"></base-input>
    <h2 class="text-5xl">Olala</h2>
  </fragment>
</template>

<script>
import BaseInput from "./BaseInput";
export default {
  components: {
    BaseInput
  },
  mounted() {
    setTimeout(() => {
      this.$refs.userInput.focusFuction();
    }, 2000);
  }
};
</script>

<style>
</style>