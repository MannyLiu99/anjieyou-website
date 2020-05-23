<template>
    <div class="banner">
      <!-- swiper -->
      <swiper :options="swiperOption" class="swiper-wrap">
        <swiper-slide class="slide-1">
            <div class="slide-tips-1">文案1</div>
            <div class="slide-tips-2">文案2</div>
            <div class="slide-tips-3">文案3</div>

        </swiper-slide>
        <swiper-slide class="slide-2">
            <div class="slide-tips-1">文案1</div>
            <div class="slide-tips-2">文案2</div>
            <div class="slide-tips-3">文案3</div>
        </swiper-slide>
        <div
          class="swiper-pagination swiper-pagination-white"
          slot="pagination"
        ></div>
      </swiper>
      <div class="particles">
        <vue-particles
            color="#dedede"
            :particleOpacity="0.7"
            :particlesNumber="80"
            shapeType="circle"
            :particleSize="4"
            linesColor="#dedede"
            :linesWidth="1"
            :lineLinked="true"
            :lineOpacity="0.4"
            :linesDistance="150"
            :moveSpeed="2"
            :hoverEffect="true"
            hoverMode="grab"
            :clickEffect="true"
            clickMode="push"
        >
        </vue-particles>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Carousel',
  data () {
    return {
      swiperOption: {
        spaceBetween: 30,
        effect: 'fade',
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        },
        autoplay: {
          delay: 3000,
          disableOnInteraction: false
        }
      }
    }
  }
}
</script>
<style scoped lang='less'>
 @import url('../assets/style/variable');
.banner{
    position: relative;
    height: 480px;

    .particles{
        width: 100%;
        height: 100%;
        overflow: hidden;
        position: absolute;
        top: 0;
        left: 0;
        z-index: 100;
    }
    .swiper-wrap{
        height: 100%;
        .swiper-slide {
            background-size: cover;
            background: #e2f2f9
                linear-gradient(
                    135deg,
                    rgba(226, 242, 249, 1) 0%,
                    rgba(224, 235, 249, 1) 49%,
                    rgba(237, 234, 249, 1) 100%
                ),
                no-repeat, center;
            color: @color-white;
            text-align: center;
            .slide-tips-1{
                font-size: 38px;
                margin-top: 120px;
            }
            .slide-tips-2{
                font-size: 32px;
                padding: 30px 0;
            }
            .slide-tips-3{
                font-size: 24px;
            }
            &.slide-1 {
                background: @color-blue-2;
            }

            &.slide-2 {
                background:@color-blue-20 ;
            }

        }
    }

}

</style>
