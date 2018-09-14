<template>
  <div>
    <nuxt/>
  </div>
</template>

<style lang="sass">
  @import url('https://fonts.googleapis.com/css?family=Noto+Sans')

  html
    font-family: "Noto Sans", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif
    font-size: 16px
    word-spacing: 1px
    -ms-text-size-adjust: 100%
    -webkit-text-size-adjust: 100%
    -moz-osx-font-smoothing: grayscale
    -webkit-font-smoothing: antialiased
    box-sizing: border-box

  *
    &:before, &:after
      box-sizing: border-box
      margin: 0

  @mixin button($color, $border-color, $hover-background-color)
    $white: #fff
    display: inline-block
    border-radius: 4px
    border: 1px solid $border-color
    color: $color
    text-decoration: none
    padding: 10px 30px
    &:hover
      color: $white
      background-color: $hover-background-color

  .button--green
    $green: #3b8070
    @include button($green, $green, $green)

  .button--grey
    $grey: #35495e
    @include button($grey, $grey, $grey)
</style>

