<template>
  <div class="btn" :class="{ primary: primary, danger: danger, info: info, warning: warning, success: success, flat: flat }">
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
    border: 1px solid transparent !important
    background-color: transparent !important
    &.primary
      color: $primary !important
      &:hover
        border: 1px solid $primary !important
    &.danger
      color: $danger !important
      &:hover
        border: 1px solid $danger !important
    &.success
      color: $success !important
      &:hover
        border: 1px solid $success !important
    &.warning
      color: $warning !important
      &:hover
        border: 1px solid $warning !important
    &.info
      color: $info !important
      &:hover
        border: 1px solid $info !important

  .primary
    color: $primary
    border: 1px solid $primary
    &:hover
      background-color: $primary
      color: #fff

  .danger
    color: $danger
    border: 1px solid $danger
    &:hover
      background-color: $danger
      color: #fff

  .success
    color: $success
    border: 1px solid $success
    &:hover
      background-color: $success
      color: #fff

  .warning
    color: $warning
    border: 1px solid $warning
    &:hover
      background-color: $warning
      color: #fff

  .info
    color: $info
    border: 1px solid $info
    &:hover
      background-color: $info
      color: #fff
</style>

<script>
  export default {
    props: {
      primary: Boolean,
      info: Boolean,
      warning: Boolean,
      danger: Boolean,
      success: Boolean,
      flat: Boolean
    }
  }
</script>