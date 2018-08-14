<template>
  <div :class="{ horizontal: horizontal, vertical: vertical }">
    <slot/>
  </div>
</template>

<style lang="sass" scoped>
  .horizontal
    display: flex
    flex-direction: row
    align-items: center
    justify-items: center

  .vertical
    display: flex
    flex-direction: column  
    align-items: center
    justify-items: center
</style>

<script>
  export default {
    props: {
      horizontal: Boolean,
      vertical: Boolean
    }
  }
</script>