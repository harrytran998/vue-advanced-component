<template>
  <fragment>
    <h1 class="text-2xl">Try to take one value of User</h1>
    <current-user>
      <template v-slot:xxx="userProp">
        {{ userProp.user.lastName }}
      </template>
    </current-user>
  </fragment>
</template>

<script>
import CurrentUser from './ScopedSlot'
export default {
  components: {
    CurrentUser,
  },
}
</script>

<style></style>
