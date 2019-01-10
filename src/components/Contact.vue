<template lang="pug">
#contact.spaced
  h1 Contact Me
  p
    ul
      li Email: {{email}}
      li Website: {{web}}
</template>

<script>
export default {
  name: 'Contact',
  data () {
    return {
      email: 'leetdavidu@gmail.com',
      web: 'leetdavid.xyz'
    }
  }
}
</script>

<style lang="sass" scoped>

</style>


