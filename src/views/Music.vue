<template>
    <main class="music" >
        <MusicPlayers />
    </main>
</template>

<script>
import MusicPlayers from '@/components/MusicPlayers.vue'

export default {
  name: 'music',
  components: {
    MusicPlayers
  }
}
</script>
