<template>
  <div class="header">
    <div class="header-left">
      <span class="iconfont">&#xe624;</span>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      {{this.city}}
      <span class="iconfont arrow-icon">&#xe612;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/variables.styl'
  .header {
    display: flex
    line-height: .86rem
    background: $bgColor
    color #fff
    text-align: center

    .header-left {
      width: .64rem
      float: left
    }
    .header-input {
      flex: 1
      height .64rem
      line-height .64rem
      margin-top .12rem
      margin-left .2rem
      background #fff
      border-radius .1rem
      color #cccccc
      text-align left
      padding-left .2rem
    }
    .header-right {
      width: 1.24rem
      float: right
      .arrow-icon {
        margin-left -.04rem
        font-size .24rem
      }
    }
  }
</style>
