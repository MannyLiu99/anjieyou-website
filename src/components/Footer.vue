<template>
  <div class="footer-box">
    <div class="content">
      <div class="footer-content">
        <div class="channel">
            <div class="name">公众号</div>
            <div class="img"></div>
        </div>
         <div class="channel">
            <div class="name">小程序</div>
            <div class="img"></div>
        </div>
        <div class="channel info-content">
          <div class="tel">XXXXXXXX</div>
          <div class="addr">
            商务合作：business@XXX.com
            <br />公司地址：XXXXX
          </div>
          <!-- <div class="footer-logo"></div> -->
        </div>
      </div>
      <footer>
        <a href="http://www.beian.miit.gov.cn" target="_blank"
          >渝ICP备XXXX号-2 <i></i>渝公网安备 XXXX号</a
        >
        <br />
        © 2019 安解忧防水有限公司. All Rights Reserved.
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style lang="less" scoped>
 @import url('../assets/style/variable');
.footer-box {
  background: #f7f9ff;
   .footer-content {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 80%;
      margin: 10px auto;
      .info-content {
        font-size: 14px;
        .tel {
          font-size: 24px;
        //   color: @font-color-active;
          padding-bottom: 10px;
        }
        .addr {
          line-height: 24px;
        }
        .footer-logo {
          width: 200px;
          height: 80px;
        // //   background: url("../assets/images/img_footer_logo.png") center
        //     no-repeat;
          background-size: 100% 100%;
          margin-top: 32px;
        }
      }
      .channel{
          margin-left: 20px;
          color: @color-green-1;
          &:first-child{
              margin-left: 0;
          }
          .name{
              text-align: center;
          }
          .img{
              width: 80px;
              height: 80px;
              background: @color-green-1;
          }
      }
    }
    footer {
      text-align: center;
      color: @color-green-5;
      font-size: 12px;
      padding: 12px 0;
      position: relative;
      &:before {
        content: "";
        display: block;
        width: 100%;
        height: 1px;
        background: linear-gradient(
          270deg,
          rgba(149, 171, 216, 0) 0%,
          @color-green-1 50%,
          rgba(149, 171, 216, 0) 100%
        );
        position: absolute;
        top: 0;
        left: 0;
      }
      a {
        color: @color-green-5;
        i {
          display: inline-block;
          width: 20px;
          height: 20px;
          line-height: 20px;
          background: url("../assets/images/icon_police.png") center no-repeat;
          background-size: 100% 100%;
          vertical-align: middle;
          margin-top: -4px;
        }
      }
    }
}
</style>
