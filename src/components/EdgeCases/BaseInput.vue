<template>
  <input type="text" ref="input" />
</template>

<script>
export default {
  methods: {
    focusFuction() {
      this.$refs.input.focus({
        preventScroll: true
      });
    }
  }
};
</script>

<style>
</style>