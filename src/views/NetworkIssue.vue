<template>
  <div>
    <h1>uh-Oh!</h1>
    <h3>
      It looks like you're experiencing some network issues. Please hit the back
      button and try again.
    </h3>
    <router-link :to="{ name: 'event-list' }">Back to Home</router-link>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped></style>
