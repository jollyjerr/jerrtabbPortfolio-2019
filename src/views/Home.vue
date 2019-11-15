<template>
  <main class="home">
    <Main />
  </main>
</template>

<script>
import Main from '@/components/Main.vue'

export default {
  name: 'home',
  components: {
    Main
  }
}
</script>

<style lang="scss">
.home {
  height: calc(100vh - 100px);
}
</style>
