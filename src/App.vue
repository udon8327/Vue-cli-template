<template lang="pug">
#app
  .container
    .wrapper
      #nav
        router-link(to="/") Home
        |  | 
        router-link(to="/about") About
      router-view
</template>

<style lang="sass">
html,body,#app
  height: 100%

body
  font-family: "Helvetica Neue", Helvetica, "PingFang TC", "LiHei Pro", "Hiragino Sans GB", "Microsoft JhengHei", "微軟正黑體", Arial ,sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  -webkit-overflow-scrolling: touch
  overflow-x: hidden
  color: #333
  background-color: #f9f9f9

p,span,h1,h2,h3,h4,h5,h6,label
  font-size: 16px
  font-weight: normal
  -webkit-text-size-adjust: none
  margin: 0
  @media (min-width: 640px)
    font-size: 18px

img
  width: 100%
  max-width: 100%
  height: auto

a
  color: #333
  text-decoration: none !important

#app
  .container
    max-width: 540px
    margin: 0 auto
    // background: url('../img/bg.jpg') repeat top center
    // background-size: 100%
    min-height: 100%
    text-align: center
    padding: 0 0 60px 0
    background-color: #fff
    .wrapper
      #nav
        a
          font-weight: bold
          color: #2c3e50
          &.router-link-exact-active
            color: #42b983

//global class
.d-none
  display: none

.animated
  animation-duration: 0.5s !important
</style>
