<template lang="pug">
  Slide
    template(v-for="navitem in navitems")
      a(v-bind:href="navitem.url")
        span
          font-awesome-icon(v-bind:icon="navitem.icon")
          |  
          | {{navitem.text}}
</template>

<script>

import { Slide } from 'vue-burger-menu'

export default {
  components: {
    Slide
  },
  data () {
    return {
      navitems: [
        {url: '#home', icon: 'home', text: 'Home'},
        {url: '#experience', icon: 'coffee', text: 'Experience'}
      ]
    }
  }
}
</script>

<style>
  .spacing {
    margin-right: 10px;
  }
  .bm-cross-button {
    right: 10px;
  }
</style>
