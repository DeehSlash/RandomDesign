<template>
  <div class="btn" :class="{ primary: primary, danger: danger, info: info, warning: warning, success: success, flat: flat, filled: filled }">
    <slot/>
  </div>
</template>

<style lang="sass" scoped>
  .btn
    height: 41px
    margin: 5px
    padding: 10px 25px
    border: 1px solid $dark
    border-radius: 5px
    background-color: transparent
    color: $dark
    box-shadow: 3px 3px 3px 0px #eee
    text-transform: uppercase
    user-select: none
    cursor: pointer
    transition: all .5s ease
    &:hover
      background-color: $dark
      color: #fff
      box-shadow: 3px 3px 3px 0px #ddd
      transition: all .15s ease
    &:active
      background-color: darken($dark, 10%)
      transition: all .15s ease

  .flat
    border: 1px solid transparent !important
    background-color: transparent !important
    color: $dark !important
    box-shadow: none !important
    &:hover
      border: 1px solid $dark !important
      box-shadow: 3px 3px 3px 0px #eee !important
    &:active
      background-color: $dark !important
      color: #fff !important
    &.primary
      color: $primary !important
      &:hover
        border: 1px solid $primary !important
      &:active
        background-color: $primary !important
        color: #fff !important
    &.danger
      color: $danger !important
      &:hover
        border: 1px solid $danger !important
      &:active
        background-color: $danger !important
        color: #fff !important
    &.success
      color: $success !important
      &:hover
        border: 1px solid $success !important
      &:active
        background-color: $success !important
        color: #fff !important
    &.warning
      color: $warning !important
      &:hover
        border: 1px solid $warning !important
      &:active
        background-color: $warning !important
        color: #fff !important
    &.info
      color: $info !important
      &:hover
        border: 1px solid $info !important
      &:active
        background-color: $info !important
        color: #fff !important

  .filled
    color: #fff !important
    background-color: $dark !important
    &:hover
      background-color: lighten($dark, 10%) !important
      border: 1px solid lighten($dark, 10%) !important
    &:active
      background-color: darken($dark, 10%) !important
    &.primary
      background-color: $primary !important
      &:hover
        background-color: lighten($primary, 10%) !important
        border: 1px solid lighten($primary, 10%) !important
      &:active
        background-color: darken($primary, 10%) !important
    &.danger
      background-color: $danger !important
      &:hover
        background-color: lighten($danger, 10%) !important
        border: 1px solid lighten($danger, 10%) !important
      &:active
        background-color: darken($danger, 10%) !important
    &.success
      background-color: $success !important
      &:hover
        background-color: lighten($success, 10%) !important
        border: 1px solid lighten($success, 10%) !important
      &:active
        background-color: darken($success, 10%) !important
    &.warning
      background-color: $warning !important
      &:hover
        background-color: lighten($warning, 10%) !important
        border: 1px solid lighten($warning, 10%) !important
      &:active
        background-color: darken($warning, 10%) !important
    &.info
      background-color: $info !important
      &:hover
        background-color: lighten($info, 10%) !important
        border: 1px solid lighten($info, 10%) !important
      &:active
        background-color: darken($info, 10%) !important

  .primary
    color: $primary
    border: 1px solid $primary
    &:hover
      background-color: $primary
      color: #fff
    &:active
      background-color: darken($primary, 10%) !important

  .danger
    color: $danger
    border: 1px solid $danger
    &:hover
      background-color: $danger
      color: #fff
    &:active
      background-color: darken($danger, 10%) !important

  .success
    color: $success
    border: 1px solid $success
    &:hover
      background-color: $success
      color: #fff
    &:active
      background-color: darken($success, 10%) !important

  .warning
    color: $warning
    border: 1px solid $warning
    &:hover
      background-color: $warning
      color: #fff
    &:active
      background-color: darken($warning, 10%) !important

  .info
    color: $info
    border: 1px solid $info
    &:hover
      background-color: $info
      color: #fff
    &:active
      background-color: darken($info, 10%) !important
</style>

<script>
  export default {
    props: {
      primary: Boolean,
      info: Boolean,
      warning: Boolean,
      danger: Boolean,
      success: Boolean,
      flat: Boolean,
      filled: Boolean
    }
  }
</script>