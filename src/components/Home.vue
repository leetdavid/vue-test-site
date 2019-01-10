<template lang="pug">
#home
  About.color-primary.spaced
  Experience.negative.spaced
  Contact.spaced
  Footer.negative.spaced
</template>

<script>

import About from '@/components/About'
import Experience from '@/components/Experience'
import Contact from '@/components/Contact'
import Footer from '@/components/Footer'

export default {
  name: 'Home',
  data() {
    return {

    }
  },
  components: {
    'About': About,
    'Experience': Experience,
    'Contact': Contact,
    'Footer': Footer
  }
}
</script>

<style lang="scss">
.color-primary {
  background: #26A69A;
}
</style>

