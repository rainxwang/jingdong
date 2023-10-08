<template>
  <div class="docker">
    <div class="docker__item docker__item--active">
      <div class="iconfont">&#xe6af;</div>
      <div class="docker__title">首页</div>
    </div>
    <div class="docker__item ">
      <div class="iconfont">&#xe600;</div>
     <div class="docker__title">购物车</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe713;</div>
      <div class="docker__title">订单</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe635;</div>
      <div class="docker__title">我的</div>
    </div>
  </div>
</template>

<style lang="scss">
.docker {
  display: flex ;
  position: absolute;
  box-sizing: border-box; //以整个box作为最外层
  padding: 0 .18rem; // 上下是0，左右有18距离
  left: 0;
  bottom: 0;
  width: 100%;
  height: .49rem;
  border-top: 1px solid #f1f1f1;
  &__item {
    flex: 1; //自适应均分等份
    text-align: center; // 文字居中
    .iconfont {
      margin: .07rem 0 .02rem 0   ;
      font-size: .2rem;
    }
    &--active {
       color: #1fa4fc;
    }
  }
  &__title {
     font-size: 20px; //web最小就是12，所以直接设置10没有效果需要使用缩放
     transform: scale(.5);
     transform-origin: center top;
  }
}
</style>
