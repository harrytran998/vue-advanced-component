<template>
  <span class="text-xl text-red-600">
    <slot :user="user">{{ user.lastName }}</slot>
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
