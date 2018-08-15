<template>
  <div class="flex" :class="{ row: row, column: column, wrap: wrap, 'justify-center': 'justify-center', 'align-center': 'align-center', 'text-center': 'text-center' }">
    <slot/>
  </div>
</template>

<style lang="sass" scoped>
  .flex
    display: flex
    flex-shrink: 0

  .row
    flex-direction: row

  .column
    flex-direction: column  

  .wrap
    flex-wrap: wrap

  .justify-center
    justify-items: center
    justify-content: center

  .align-center
    align-items: center
    align-content: center

  .text-center
    text-align: center
</style>

<script>
  export default {
    props: {
      row: Boolean,
      column: Boolean,
      wrap: Boolean,
      'justify-center': Boolean,
      'align-center': Boolean,
      'text-center': Boolean
    }
  }
</script>