<template>
  <section class="container full">
    <btn primary>Primary</btn>
    <btn info>Info</btn>
    <btn success>Success</btn>
    <btn warning>Warning</btn>
    <btn danger>Danger</btn>
    <br>
    <card>
      <card-title>Lorem Ipsum</card-title>
      <card-content>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </card-content>
      <card-actions>
        <btn danger flat>Cancel</btn>
        <btn primary flat>Ok</btn>
      </card-actions>
    </card>
  </section>
</template>

<style lang="sass" scoped>
  .container
    display: flex
    flex-direction: column
    justify-content: center
    align-items: center
    text-align: center

  .full
    width: 100%
    height: 100%
</style>

<script>
  import Btn from '~/components/Btn'
  import Card from '~/components/Card'
  import CardTitle from '~/components/CardTitle'
  import CardContent from '~/components/CardContent'
  import CardActions from '~/components/CardActions'

  export default {
    components: {
      Btn, Card, CardTitle, CardContent, CardActions
    }
  }
</script>
