<template>
    <div class="nav-box">
        <div class="logo" >{{message}}</div>
        <div class="nav-wrap">
            <div class="nav-item active">首页</div>
            <div class="nav-item">关于我们</div>
            <div class="nav-item">成功案例</div>
            <div class="nav-item">技术答疑</div>
            <div class="nav-item">联系我们</div>
        </div>
    </div>
</template>

<script>
export default {
  data () {
    return {
      message: '安解忧logo'
    }
  }
}
</script>
<style scoped lang='less'>
@import url('../assets/style/variable');

.nav-box{
    background: @color-green-3;
    color: @color-white;
    display: flex;
    align-items: center;
    justify-content: space-around;
    position: fixed;
    z-index: 999;
    top: 0;
    right: 0;
    left: 0;
    font-size: 22px;
    height: @nav-height;
    .nav-wrap{
        display: flex;
        align-items: center;
        justify-content: space-around;
         height: @nav-height;
        .nav-item{
            padding: 0 50px;
            height: @nav-height;
            line-height: @nav-height;
            &:hover{
                background: @color-green-1;
            }
        }
        .nav-item.active{
            position: relative;
            &::after{
                content: '';
                display: block;
                width: 100%;
                height: 4px;
                background: @color-green-1;
                position: absolute;
                bottom: 0;
                left: 0;
            }
        }
    }
}
</style>
