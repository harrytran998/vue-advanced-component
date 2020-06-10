<template>
  <span>
    <slot :user="user" class="name">{{ user.lastName }}</slot>
  </span>
</template>

<script>
export default {
  name: 'CurrentUser',
  data: () => ({
    user: {
      firstName: 'Fuck',
      lastName: 'Boy',
    },
  }),
}
</script>

<style>
.name {
  font-size: 2.5rem;
}
</style>
