<template>
  <div class="home-page primary">
    <AppWrapper />
  </div>
</template>

<script>
import AppWrapper from '~/components/Home/AppWrapper'
export default {
  components: {
    AppWrapper
  }
}
</script>

<style lang="scss">
.home-page {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
