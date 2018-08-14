<template>
  <div class="card">
    <slot/>
  </div>
</template>

<style lang="sass" scoped>
  .card
    min-height: 25px
    width: 400px
    margin: 5px
    padding: 20px 15px
    border-radius: 5px
    border: 1px solid #eee
    box-shadow: 15px 15px 15px 0px #eee
</style>
