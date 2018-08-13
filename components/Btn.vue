<template>
  <div class="btn" :class="{ primary: isPrimary, danger: isDanger, info: isInfo, warning: isWarning, success: isSuccess, flat: isFlat }">
    <slot/>
  </div>
</template>

<style lang="sass" scoped>
  .btn
    margin: 5px
    padding: 10px 25px
    border-radius: 5px
    background-color: transparent
    text-transform: uppercase
    user-select: none
    transition: all .5s ease
    &:hover
      transition: all .15s ease

  .flat
    border: none !important
    &:hover
      background-color: transparent !important
      background-color: #efefef !important
    &.primary
      color: #5f1c8b !important
    &.danger
      color: red !important
    &.success
      color: green !important
    &.warning
      color: orange !important
    &.info
      color: blue !important


  .primary
    color: #5f1c8b
    border: 1px solid #5f1c8b
    &:hover
      background-color: #5f1c8b
      color: #fff

  .danger
    color: red
    border: 1px solid red
    &:hover
      background-color: red
      color: #fff

  .success
    color: green
    border: 1px solid green
    &:hover
      background-color: green
      color: #fff

  .warning
    color: orange
    border: 1px solid orange
    &:hover
      background-color: orange
      color: #fff

  .info
    color: blue
    border: 1px solid blue
    &:hover
      background-color: blue
      color: #fff
</style>

<script>
  export default {
    props: ['primary', 'info', 'warning', 'danger', 'success', 'flat'],

    computed: {
      isPrimary () {
        return this.primary !== undefined
      },

      isDanger () {
        return this.danger !== undefined
      },

      isInfo () {
        return this.info !== undefined
      },

      isWarning () {
        return this.warning !== undefined
      },

      isSuccess () {
        return this.success !== undefined
      },

      isFlat () {
        return this.flat !== undefined
      }
    }
  }
</script>