<template lang="pug">
#experience
  h1 Experience
  .container
    .text-left.black(v-for="card in cards")
      b-card(
        v-bind:title="card.title"
        v-bind:img-src="card.imgsrc"
        img-alt="Image"
        img-top
        tag="article"
        style="max-width: 20rem;"
        class="mb-2"
      )
        p.card-text: b {{card.jobtitle}}
        p.card-text {{card.desc}}
        b-button(
          v-bind:href="card.url"
          variant="primary"
        ) Learn More
    template(v-for="carddd in cards2")
      Card(:card="carddd")
</template>

<script>

import Card from '@/components/Card'

export default {
  name: 'Experience',
  data() {
    return {
      cards: [
        {
          title: 'HSBC',
          imgsrc: require('@/assets/img/hsbc.jpg'),
          jobtitle: 'Industrial Placement Trainee',
          desc: 'Work description goes here',
          url: '/experience/#hsbc'
        }
      ],
      cards2: [
        {
          url: '#',
          image: require('@/assets/img/hsbc.jpg'),
          company: 'HSBC',
          jobtitle: 'Industrial Placement Trainee',
          desc: 'Work description goes here',
          author: 'Learn More'
        }
      ]
  } },
  components: {
    'Card': Card
  }
}
</script>

<style lang="scss" scoped>
</style>
