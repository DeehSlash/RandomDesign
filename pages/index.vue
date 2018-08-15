<template>
  <section class="container full">
    <h1>Button</h1>
    <align horizontal>
      <btn primary>Primary</btn>
      <btn info>Info</btn>
      <btn success>Success</btn>
      <btn warning>Warning</btn>
      <btn danger>Danger</btn>
    </align>

    <h1>Button (Filled)</h1>
    <align horizontal>
      <btn primary filled>Primary</btn>
      <btn info filled>Info</btn>
      <btn success filled>Success</btn>
      <btn warning filled>Warning</btn>
      <btn danger filled>Danger</btn>
    </align>

    <h1>Button (Flat)</h1>
    <align horizontal>
      <btn primary flat>Primary</btn>
      <btn info flat>Info</btn>
      <btn success flat>Success</btn>
      <btn warning flat>Warning</btn>
      <btn danger flat>Danger</btn>
    </align>

    <br>
    <card>
      <card-title>Lorem Ipsum</card-title>
      <card-content>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
      </card-content>
      <card-actions>
        <btn flat>Cancel</btn>
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
  import Align from '~/components/Align'
  import Btn from '~/components/Btn'
  import Card from '~/components/Card'
  import CardTitle from '~/components/CardTitle'
  import CardContent from '~/components/CardContent'
  import CardActions from '~/components/CardActions'

  export default {
    components: {
      Align, Btn, Card, CardTitle, CardContent, CardActions
    }
  }
</script>
