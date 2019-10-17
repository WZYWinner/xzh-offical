<template>
  <div id="JobChance">
    <div class="banner container-fuild text-center">招商简介</div>
    <div class="advantage"></div>
    <div class="row">
      <div class="col-xs-3 wow zoomInLeft"><div class="introduce1"><p>支付方式不断变革</p></div></div>
      <div class="col-xs-3 wow zoomInLeft"><div class="introduce2"><p>智能技术不断升级</p></div></div>
      <div class="col-xs-3 wow zoomInRight"><div class="introduce3"><p>市场规模逐日庞大</p></div></div>
      <div class="col-xs-3 wow zoomInRight"><div class="introduce4"><p>公司体系制度完善</p></div></div>
    </div>
    <div class="container">
      <!-- PC -->
      <div class="info">
        <div class="part">
          <div class="icon1 icon wow zoomIn"></div>
          <div class="text1 text"><p>全面支持</p><p>合作伙伴从合同签订成功之日起，从员工培训到整体运营为合作伙伴管理好团队提供全面支持！</p></div>
        </div>
        <div class="part">
          <div class="icon2 icon wow zoomInRight"></div>
          <div class="text2 text"><p>专属管家</p><p>专业资深的客服团队一对一全程指导，从下到线上所有流程无限次指导，指导学会为止。</p></div>
        </div>
        <div class="part">
          <div class="icon3 icon wow zoomIn"></div>
          <div class="text3 text"><p>技术支持</p><p>技术团队来自国内顶尖IT公司，能在技术上给予合作伙伴强大的保障。</p></div>
        </div>
        <div class="part">
          <div class="icon4 icon wow zoomInLeft"></div>
          <div class="text4 text"><p>运营支持</p><p>芯智汇拥有强大的运营团队定期进行业务指导，协助合作伙伴进行市场开拓。</p></div>
        </div>
        <div class="part">
          <div class="icon5 icon wow zoomIn"></div>
          <div class="text5 text"><p>产品共享</p><p>合作伙伴将在定制专属网页网站、APP、微信平台、小程序、金融行业软件等内容可享受各类内部优惠。</p></div>
        </div>
      </div>
      <!-- 移动 -->
      <div class="mobile">
        <div class="part">
          <div class="icon1 icon wow zoomIn"></div>
          <div class="text1 text"><p>全面支持</p><p>合作伙伴从合同签订成功之日起，从员工培训到整体运营为合作伙伴管理好团队提供全面支持！</p></div>
        </div>
        <div class="part">
          <div class="icon2 icon wow zoomInRight"></div>
          <div class="text2 text"><p>专属管家</p><p>专业资深的客服团队一对一全程指导，从下到线上所有流程无限次指导，指导学会为止。</p></div>
        </div>
        <div class="part">
          <div class="icon3 icon wow zoomIn"></div>
          <div class="text3 text"><p>技术支持</p><p>技术团队来自国内顶尖IT公司，能在技术上给予合作伙伴强大的保障。</p></div>
        </div>
        <div class="part">
          <div class="icon4 icon wow zoomInLeft"></div>
          <div class="text4 text"><p>运营支持</p><p>芯智汇拥有强大的运营团队定期进行业务指导，协助合作伙伴进行市场开拓。</p></div>
        </div>
        <div class="part">
          <div class="icon5 icon wow zoomIn"></div>
          <div class="text5 text"><p>产品共享</p><p>合作伙伴将在定制专属网页网站、APP、微信平台、小程序、金融行业软件等内容可享受各类内部优惠。</p></div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { WOW } from 'wowjs';
export default {
  name: "JobChance",
  data() {
    return {};
  },
  mounted(){
    var wow = new WOW();
    wow.init();
  }
};
</script>
<style scoped>
.banner {
  color: #fff;
  font-size: 30px;
  height: 150px;
  line-height: 150px;
  background-image: url("../assets/img/banner_2.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: scroll;
  background-position: center center;
}
.JobChance-container {
  margin: 100px;
  padding: 30px;
  transition: all ease 0.5s;
  border: 1px dashed salmon;
}
.JobChance-container h2{
  color: rgb(255, 102, 19);
  font-weight: bolder;
  text-align: center;
}
.JobChance-container p{
font-size: 20px;
  color: rgb(255, 102, 19);
  font-weight: 700;
}
.JobChance-container ol{
    list-style-type: decimal;
    padding-left: 30px;
}
.JobChance-container ol>li{
    font-size: 14px;
    line-height: 2.7rem;
}@media screen and (min-width: 997px) {
  .info{
    display: block;
  }
  .mobile {
		display: none;
	}
}
@media screen and (max-width: 997px) {
  .info{
    display: none;
  }
  .mobile {
		display: block;
	}
  .container{
    width: 600px;
  }
  .JobChance-container {
    margin: 20px 0;
    padding: 20px;
    border: 1px dashed salmon;
  }
  .mobile{
  width: 100%;
  height: 600px;
  background-image: url(../assets/img/Screen.png);
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: scroll;
  background-position: center center;
  position: relative;
}
.mobile .part{
  position: relative;
}
.mobile .icon1{
  position: absolute;
  background: url(../assets/img/icon1.png);
  background-size: 100%;
  left: 50px;
  top: 100px;
  z-index: 999;
}
.mobile .icon2{
  position: absolute;
  background: url(../assets/img/icon2.png);
  background-size: 100%;
  left: 40px;
  top: 380px;
  z-index: 999;
}
.mobile .icon3{
  position: absolute;
  background: url(../assets/img/icon3.png);
  background-size: 100%;
  left: 280px;
  top: 380px;
  z-index: 999;
}
.mobile .icon4{
  position: absolute;
  background: url(../assets/img/icon4.png);
  background-size: 100%;
  left: 420px;
  top: 300px;
  z-index: 999;
}
.mobile .icon5{
  position: absolute;
  background: url(../assets/img/icon5.png);
  background-size: 100%;
  left: 460px;
  top: 140px;
  z-index: 999;
}
.mobile .icon{
  height: 65px;
  width: 65px;
}
.mobile .text1{
  background-color: rgb(0, 0, 0,0.7);
  position: absolute;
  left: 90px;
  top: 140px;
}
.mobile .text2{
  background-color: rgb(0, 0, 0,0.7);
  position: absolute;
  left: 80px;
  top: 420px;
}
.mobile .text3{
  background-color: rgb(0, 0, 0,0.7);
  position: absolute;
  left: 320px;
  top: 420px;
}
.mobile .text4{
  background-color: rgb(0, 0, 0,0.7);
  position: absolute;
  left: 460px;
  top: 220px;
}
.mobile .text5{
  background-color: rgb(0, 0, 0,0.7);
  position: absolute;
  left: 500px;
  top: 60px;
}
.mobile .part .text{
  width: 200px;
  height: 100px;
  padding: 10px;
  font-size: 5px;
  text-align: center;
  color: white;
  display: none;
  animation: mymove 1s;
}
@keyframes mymove{
  from{
    opacity: 0;
  }
  to{
    opacity: 1;
  }
}
.mobile .part:hover .text{
  display: block;
}
}
/* .content{
  width: 1300px;
    margin: 0 auto;
    margin-bottom: 20px;
} */
.info{
  width: 100%;
  height: 600px;
  background-image: url(../assets/img/Screen.png);
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: scroll;
  background-position: center center;
  position: relative;
}
.info .part{
  position: relative;
}
.info .icon1{
  position: absolute;
  background: url(../assets/img/icon1.png);
  background-size: 100%;
  left: 180px;
  top: 40px;
  z-index: 999;
}
.info .icon2{
  position: absolute;
  background: url(../assets/img/icon2.png);
  background-size: 100%;
  left: 220px;
  top: 300px;
  z-index: 999;
}
.info .icon3{
  position: absolute;
  background: url(../assets/img/icon3.png);
  background-size: 100%;
  left: 480px;
  top: 450px;
  z-index: 999;
}
.info .icon4{
  position: absolute;
  background: url(../assets/img/icon4.png);
  background-size: 100%;
  left: 760px;
  top: 350px;
  z-index: 999;
}
.info .icon5{
  position: absolute;
  background: url(../assets/img/icon5.png);
  background-size: 100%;
  left: 860px;
  top: 140px;
  z-index: 999;
}
.info .icon{
  height: 80px;
  width: 80px;
}
.info .text1{
  background-color: rgb(0, 0, 0,0.7);
  
  position: absolute;
  left: 220px;
  top: 100px;
}
.info .text2{
  background-color: rgb(0, 0, 0,0.7);
  position: absolute;
  left: 260px;
  top: 360px;
}
.info .text3{
  background-color: rgb(0, 0, 0,0.7);
  position: absolute;
  left: 530px;
  top: 370px;
}
.info .text4{
  background-color: rgb(0, 0, 0,0.7);
  position: absolute;
  left: 580px;
  top: 270px;
}
.info .text5{
  background-color: rgb(0, 0, 0,0.7);
  position: absolute;
  left: 910px;
  top: 190px;
}
.info .part .text{
  width: 220px;
  height: 100px;
  padding: 10px;
  font-size: 12px;
  text-align: center;
  color: white;
  display: none;
  animation: mymove 1s;
}
@keyframes mymove{
  from{
    opacity: 0;
  }
  to{
    opacity: 1;
  }
}
.info .part:hover .text{
  display: block;
}
.advantage{
  background: url(../assets/img/advantage_1.png) no-repeat;
  width: 300px;
  height: 57px;
  background-size: 100%;
  margin: 50px auto;
}
.row{
  text-align: center;
  padding: 6% 15%;
}
.introduce1{
  width: 93%;
  background: url(../assets/img/advantage1.png);
  background-size: 100%;
}
.introduce2{
  width: 93%;
  background: url(../assets/img/advantage2.png);
  background-size: 100%;
}
.introduce3{
  width: 93%;
  background: url(../assets/img/advantage3.png);
  background-size: 100%;
}
.introduce4{
  width: 93%;
  background: url(../assets/img/advantage4.png);
  background-size: 100%;
}
.introduce1 p{
  padding-top: 94%;
  color: #fff;
}
.introduce2 p{
  padding-top: 94%;
  color: #fff;
}
.introduce3 p{
  padding-top: 94%;
  color: #fff;
}
.introduce4 p{
  padding-top: 94%;
  color: #fff;
}
</style>

