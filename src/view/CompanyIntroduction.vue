<template>
    <div id="CompanyIntroduction">
        <div class="banner container-fuild text-center">关于我们</div>
        <div class="container">
            <div class="row CompanyIntroduction-container">
                <div class="col-xs-12 col-sm-12 col-md-6 wow zoomIn">
                    <img class="img-responsive center-block" src="@/assets/img/about_img.png">
                </div>
                <div class="col-xs-12 col-sm-12 col-md-6">
                    <h3>公司简介</h3>
                    <p class=".text-justify">福建芯智汇信息技术有限公司、创立于2018 年 07 月 04 日。是一家集成民生信用综合服务、电子系统开发及应用、网络与信息安全软件开发、应用软件开发、智能化管理系统开发与应用为一体的高新技术企业。拥有一批从事本专业10余年从业经验的专业团队。</p>
                    <p class=".text-justify">公司打造“芯智汇”APP，结合智能与专业的客服服务进行银行积分兑换，实现帮助持卡人用卡进行信息管理及个人财产智能化应用。芯智汇APP还具备信用卡申请、贷款申请、卡医生（信用卡用卡情况评估）、征信查询、用卡知识普及、商户收款等多项民生与信用相结合的功能。目前在芯智汇APP上可进行建设、工商、中国、招商、平安、光大、北京等 26 家全国性银行及 30 余家地方银行的积分兑换。更多银行项目正在接洽中，将陆续上线。</p>
                </div>
            </div>
            <div class="company_concept"><img src="../assets/img/company_concept.png" alt=""></div>
            <div class="concept">
			<div class="row">
				<div class="content col-xs-12 col-sm-4 .col-md-4 wow slideInRight">
					<div class="concepts1 grow">
						<h4>芯智汇理念</h4>
						<p>坚持以“用户为本，最大程度满足用户需求，优化用户体验”的经营理念做到信用卡服务您的生活，芯智汇服务您的财富。</p>
					</div>
				</div>
				<div class="content col-xs-12 col-sm-4 .col-md-4 wow slideInRight">
					<div class="concepts2 grow">
						<h4>芯智汇实力</h4>
						<p>公司拥有最专业的技术团队，雄厚的资金链支持、上百位运营经理、数千名代理商规模、在信用卡服务领域独占鳌头。</p>
					</div>
				</div>
				<div class="content col-xs-12 col-sm-4 .col-md-4 wow slideInRight">
					<div class="concepts3 grow">
						<h4>芯智汇宗旨</h4>
						<p>公司打造“芯智汇APP”结合智能与专业的客服服务， 帮助用户解决各类持卡问题，及实现个人财产智能化应用管理。</p>
					</div>
				</div>
			</div>
		</div>
        </div>
    </div>
</template>
<script>
import { WOW } from 'wowjs';
export default {
    name: 'CompanyIntroduction',
    data(){
        return{

        }
    },
    mounted(){
        var wow = new WOW();
        wow.init();
    }
}
</script>
<style scoped>
.banner{
    color: #fff;
    font-size: 30px;
    height: 150px;
    line-height: 150px;
    background-image: url('../assets/img/banner1.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: scroll;
    background-position: center center;
}
.row{
    margin-right: 0;
    margin-left: 0;
}
.company_concept{
    width: 300px;
    margin: 30px auto;
}
.company_concept img{
    width: 300px;
}
.concept {
	margin-bottom: 50px;
}

.concept .row .content .concepts1,
.concept .row .content .concepts2,
.concept .row .content .concepts3 {
	width: 90%;
	overflow: hidden;
	background: url(../assets/img/concept.png) no-repeat;
	background-size: 100%;
	-webkit-box-shadow: 0px 5px 10px rgba(102, 102, 102, 0.6);
	box-shadow: 0px 5px 10px rgba(102, 102, 102, 0.6);
	padding-bottom: 45px;
	margin-left: 5%;
	background-color: #fafafa !important;
}

.concept .row .content .concepts2 {
	background: url(../assets/img/power.png) no-repeat;
	background-size: 100%;
}

.concept .row .content .concepts3 {
	background: url(../assets/img/objective.png) no-repeat;
	background-size: 100%;
}

.concepts1,
.concepts2,
.concepts3 {
	text-align: center;
	padding: 0 16px;
}

.concepts1 h4,
.concepts2 h4,
.concepts3 h4 {
	padding-top: 60%;
}

.concepts1 p,
.concepts2 p,
.concepts3 p {
	text-indent: inherit !important;
	font-size: 14px;
	padding-top: 20px;
}
.CompanyIntroduction-container{
    padding: 100px 0;
    color: #808080;
    transition: all ease 0.5s;
}
.CompanyIntroduction-container>div>p{
    font-size: 14px;
    line-height: 2.5rem;
}
@media screen and (max-width: 997px){
    .CompanyIntroduction-container{
    padding: 10px 0;
    color: #808080;
}
}
</style>

