<template>
  <fragment>
    <h1 class="text-2xl">Try to take one value of User</h1>
    <current-user>
      <template #name="{ user: { firstName, lastName } }">{{ firstName + ' ' + lastName }}</template>
      <template #age="{ user }">{{ user.age }}</template>
    </current-user>
    <h2>{{ getInforParent() }}</h2>
  </fragment>
</template>

<script>
import CurrentUser from "./ScopedSlot";
export default {
  components: {
    CurrentUser
  },
  methods: {
    getInforParent() {
      console.log(this.$children);
      return this.$parent.user.age;
    }
  }
};
</script>

<style></style>
