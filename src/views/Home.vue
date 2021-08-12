<template>
  <div class="container">
    <item v-for="story in stories" :key="story.data.id" :story="story"></item>
    <hr>
    <Footer />
  </div>
</template>

<script>
import Item from '@/views/Item.vue'
import Footer from '../components/Footer.vue'

export default {
  name: 'home',
  components: {
    'item': Item,
    Footer
    

  },
  data() {
    return {
      err: '',
      stories: this.$store.state.topStories
    }
  },
  created() {
    if (this.$store.state.topStories.length === 0) this.$store.dispatch('fetch_top_stories')
  }
}
</script>
<style>
hr {
  background-color:#006d77;
}
</style>
