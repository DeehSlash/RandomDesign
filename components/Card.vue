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
    border: 1px solid #ccc
    border-radius: 5px
    background-color: #fafafa
</style>
