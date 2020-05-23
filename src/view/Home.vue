<template>
    <div class="content">
       <navigation></navigation>
       <div class="wrap">
        <home-banner></home-banner>
        <div class="section">
          <div class="section-img">图片</div>
          <div class="section-txt">防水工程施工,涂装工程施工(以上两项范围涉及许可的,均需取得相关行政许可后方可经营);销售:建筑材料、装饰材料(以上两项不含危化品)、防水防腐材料、五金交电。**【以上经营范围依法须经批准的项目,经相关部门批准后方可开展经营活动】</div>
        </div>
        <div class="section">
          <div class="section-txt">防水工程施工,涂装工程施工(以上两项范围涉及许可的,均需取得相关行政许可后方可经营);销售:建筑材料、装饰材料(以上两项不含危化品)、防水防腐材料、五金交电。**【以上经营范围依法须经批准的项目,经相关部门批准后方可开展经营活动】</div>
          <div class="section-img">图片</div>
        </div>

        <div>色块测试</div>
        <div class="color-test">
            <div class="item" style="background: rgba(83,97,84,1)">@color-green-1</div>
            <div class="item"  style="background: rgba(99,110,93,1);">@color-green-2</div>
            <div class="item"  style="background: rgba(140,152,140,1);">@color-green-3</div>
            <div class="item"  style="background: rgba(167,174,158,1);">@color-green-4</div>
            <div class="item"  style="background: rgba(72,108,98,1);">@color-green-5</div>
            <div class="item"  style="background: rgba(82,112,114,1)">@color-green-6</div>
            <div class="item"  style="background: rgba(153,191,178,1);">@color-green-7</div>

            <div class="item"  style="background: rgba(201,216,223,1);">@color-blue-1</div>
            <div class="item"  style="background: rgba(106,144,147,1)">@color-blue-2</div>
            <div class="item"  style="background: rgba(35,51,67,1)">@color-blue-3</div>
            <div class="item"  style="background: rgba(74,90,105,1);">@color-blue-4</div>
            <div class="item"  style="background: rgba(165,175,187,1);">@color-blue-5</div>
            <div class="item"  style="background: rgba(79,115,132,1);">@color-blue-20</div>
        </div>
       </div>
       <Footer></Footer>
    </div>
</template>

<script>
import Navigation from '@/components/Navigation'
import HomeBanner from '@/components/HomeBanner'
import Footer from '@/components/Footer'
// import Footer from '@/components/Footer'
export default {
  components: {
    Navigation,
    HomeBanner,
    Footer
  },
  data () {
    return {
      message: 'hhhhh'
    }
  }
}
</script>
<style scoped lang="less">
@import url('../assets/style/variable');
.color-test{
  display: flex;
  .item{
    width: 100px;
    height: 100px;
  }
}
.section{
  display: flex;
  justify-content: space-between;
  // align-items: center;
  margin: 22px 0;
  .section-img{
    width: 800px;
    height: 400px;
    background: @color-blue-2;
  }
  .section-txt{
    flex: 1;
    font-size: 18px;
    line-height: 30px;
  }
  &>:first-child{
    margin-right: 22px;
  }
}

</style>
