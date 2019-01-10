<template lang="pug">
#about.spaced
  h1 {{name}}
    | 
    b ({{nickname}})
  p {{desc}}
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      name: 'LEE, Eun Shang',
      nickname: 'David',
      desc: 'Programmer, Solidity Developer, Technology Enthusiast'
    }
  }
}
</script>

<style lang="sass" scoped>
  
</style>
