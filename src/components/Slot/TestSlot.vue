<template>
  <fragment>
    <current-user>
      <template v-slot="userProp">
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
