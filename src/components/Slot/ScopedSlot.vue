<template>
  <span class="text-xl text-red-600">
    <slot name="name" :user="user"></slot>
    <slot name="age" :user="user"></slot>
  </span>
</template>

<script>
export default {
  name: "CurrentUser",
  data: () => ({
    user: {
      firstName: "Fuck",
      lastName: "Boy",
      age: 20
    }
  })
};
</script>
