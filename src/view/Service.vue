<template>
    <div id="Service">
        <div class="container text-center">
            <h3>我们的服务</h3>
            <p style="color:#b2b2b2">The Best Service You Never See</p>
        </div>
        <div class="container">
            <div class="Service-container row">
                <!-- v-for="(item,index) in serviceList" :key="index" @click="ServiceClick(item.id)"> -->
                <div class="Service-item col-xs-12 col-sm-6 col-md-3 wow slideInUp" 
                v-for="(item,index) in serviceList" :key="index">
                    <div class="Service-item-wrapper">
                        <div class="Service-item-top">
                            <h4>{{item.title}}</h4>
                            <i></i>
                            <p>{{item.eng_title}}</p>
                        </div>
                        <div class="Service-item-img">
                            <img :src="item.img" alt="服务">
                        </div>
                        <div class="Service-item-border"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import { WOW } from 'wowjs';
export default {
    name: 'Service',
    data(){
        return{
            serviceList: [
                {
                    id: 'section-1',
                    title: '刷脸支付软硬件',
                    eng_title: '刷脸支付打通第三方支付系统、会员营销系统、微信小程序、打赏、大屏互动等新媒体互动应用及相关硬件设备，适用于各个行业。以刷脸为切入点，为商家提供合理的移动支付解决方案。',
                    img: require('@/assets/img/service1.jpg')
                },{
                    id: 'section-2',
                    title: '人脸智能云平台',
                    eng_title: '对入店客户进行精准分析，包括性别、年龄、表情等，帮助门店全面掌握 用户画像，精准服务目标客户。',
                    img: require('@/assets/img/service2.jpg')
                },{
                    id: 'section-3',
                    title: '会员智能云平台',
                    eng_title: '精准客群管理，建立门店专属会员库，进行定制化区别营销，全面提升消费体验和购买转化，促进服务价值变现。',
                    img: require('@/assets/img/service3.jpg')
                },{
                    id: 'section-4',
                    title: '智能互动摄像头',
                    eng_title: '智能摄像头，通过智能算法自动追踪人脸，快速捕捉人脸图像， 可同步与多人进行AR互动，根据识别的客户属性，自动推荐商品或发送优惠券。',
                    img: require('@/assets/img/service4.jpg')
                }
            ]
        }
    },
    mounted(){
        var wow = new WOW();
        wow.init();
    },
    methods:{
        ServiceClick(id){
            this.$router.push({
                name: 'servicedetail',
                params: {
                    id: id
                }
            })
        }
    }
}
</script>
<style scoped>
.Service-container{
    padding: 30px 50px;
}
.Service-item{
    margin-bottom: 50px;
}
.Service-item-wrapper{
    cursor: pointer;
    background: rgba(244,244,244,1);
    overflow: hidden;
    position: relative;
}
.Service-item-top{
    width: 100%;
    height: 120px;
    padding: 30px;
    text-align: center;
}
.Service-item-top>i{
    display: inline-block;
    width: 25px;
    height: 2px;
    background: #28f;
}
.Service-item-top>p{
    color: #474747;
    opacity: 0;
    transform: translateY(10px);
    transition: all .5s ease;
    margin-top: 20px;
}
.Service-item-img{
    width: 100%;
    overflow: hidden;
}
.Service-item-img img{
    width: 100%;
    transition: all 0.5s ease;
}
.Service-item-border{
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    margin: auto;
    z-index: 9999999;
    width: 100%;
    height: 100%;
    transition: all 0.5s ease;
    border: 1px solid #000;
    opacity: 0;
}
.Service-item-wrapper:hover .Service-item-top > i{
    opacity: 0;
}
.Service-item-wrapper:hover .Service-item-top > p{
    opacity: 1;
    /* transform: translateY(-10px); */
}
.Service-item-wrapper:hover .Service-item-img > img{
    /* transform: scale(1.1,1.1); */
    opacity: 0;
}
.Service-item-wrapper:hover > .Service-item-border{
    opacity: 1;
    width: 90%;
    height: 90%;
}
</style>

