<template>
    <div>
      <home-menu-bar />
      <el-row>
        <div class="block">
          <el-carousel height="500px" >
            <el-carousel-item v-for="item in imgArr" :key="item">
              <div :style="{backgroundImage:'url('+item+')'}" >  </div>
            </el-carousel-item>
          </el-carousel>
        </div>
      </el-row>
      <!--交易步骤 -->
      <el-row style="margin-top: 50px">
        <h1 style="font-weight: 100">买车流程</h1>
      </el-row>
      <el-row>
        <el-col :span="12" :offset="6">
          <el-steps :align-center="true">
            <el-step title="付定金"></el-step>
            <el-step title="发货"></el-step>
            <el-step title="交尾款"></el-step>
            <el-step title="提车"></el-step>
          </el-steps>
        </el-col>
      </el-row>
      <el-row class="compInfo">
          <el-col :span="4" :offset="12" class="text1">106个城市</el-col>
          <el-col :span="4" :offset="-6" class="text1">138个服务中心</el-col>
          <el-col :span="20" :offset="4" class="text2">专业的基础设施，极致的卖车服务</el-col>
      </el-row>
      <el-row style="margin-top: 80px">
        <el-col :span="6">
          <h1>30,000+</h1>
          <span style="width: 10px">
            3万多库存车，随订随发
          </span>
        </el-col>
        <el-col :span="6">
          <h1>10,000+</h1>
          <span>
            直接合作厂家一万多家，谁家便宜拿谁家
          </span>
        </el-col>
        <el-col :span="6">
          <h1>权威大数据</h1>
          <span>
            全网最权威大数据为您估价，不让您多花一分钱
          </span>
        </el-col>
        <el-col :span="6">
          <h1>省时省心</h1>
          <span>
            一站式交易，方便快捷省时省心
          </span>
        </el-col>
      </el-row>
      <!--金牌服务-->
      <el-row class="gold_service">
        <el-col style="height: 160px;margin-top: -30px"><h1>金牌服务</h1></el-col>
        <el-col :span="5" :offset="2" class="gold_service_space">
          <div class="gold_service_content">
            <div class="gold_service_content_1"><img src="../../static/images/car.png" alt="" style="width: 60px"></div>
            <div class="gold_service_content_box">
              <div class="gold_service_content_2">当天发车</div>
              <div class="gold_service_content_3">收订金后24h内闪电发车</div>
            </div>
          </div>
        </el-col>
        <el-col :span="5" class="gold_service_space">
          <div class="gold_service_content">
            <div class="gold_service_content_1"><img src="../../static/images/price.png" alt=""></div>
            <div class="gold_service_content_box">
            <div class="gold_service_content_2">正品保证</div>
            <div class="gold_service_content_3">货源厂家直供,保证品质</div>
            </div>
          </div>
        </el-col>
        <el-col :span="5" class="gold_service_space">
          <div class="gold_service_content">
            <div class="gold_service_content_1"><img src="../../static/images/heart.png" alt=""></div>
            <div class="gold_service_content_box">
            <div class="gold_service_content_2">全程托管</div>
            <div class="gold_service_content_3">全程GPS跟踪,专人负责</div>
            </div>
          </div>
        </el-col>
        <el-col :span="5" class="gold_service_space">
          <div class="gold_service_content">
            <div class="gold_service_content_1"><img src="../../static/images/service.png" alt=""></div>
            <div class="gold_service_content_box">
            <div class="gold_service_content_2">7*24h服务</div>
            <div class="gold_service_content_3">售前、售中、售后7*24服务</div>
            </div>
          </div>
        </el-col>
      </el-row>
        <el-row >
          <el-col class="car_story_title">
            车主故事
          </el-col>
          <el-col :span="10" :offset="4">
            <div class="car_story">
              <div class="car_story_img" style="background-position: 0 -640px" ></div>
                <div class="car_story_content">
                  <div class="car_story_content_1">李先生 | 培训师 | 标致</div>
                  <div class="car_story_content_2">
                    朋友介绍知道的除了4S店还有别的渠道可以买车。抱着试一试的想法，和兵丰远达的服务人员沟通后，买到了心满意足的车。
                  </div>
                </div>
            </div>
          </el-col>
          <el-col :span="10" >
            <div class="car_story">
              <div class="car_story_img" style="background-position: 0 -480px" ></div>
              <div class="car_story_content">
                <div class="car_story_content_1">乔先生 | 种子批发商 | 别克</div>
                <div class="car_story_content_2">
                  兵丰远达诚信、用心、速度、质量。便捷了买车的朋友们。时间就是金钱，为客户省下了大把时间。我信赖兵丰远达。祝愿兵丰远达越来越好，你们是客户的福音！
                </div>
              </div>
            </div>
          </el-col>
          <el-col :span="10" :offset="4">
            <div class="car_story">
              <div class="car_story_img" style="background-position: 0 -960px" ></div>
              <div class="car_story_content">
                <div class="car_story_content_1">王女士 | 大学老师 | 雪佛兰</div>
                <div class="car_story_content_2">
                  在网上看到车置宝的信息，抱着尝试的态度咨询了一下，客服态度很好，检测师上门检测，小哥很精神也很专业，好感度瞬间增加，卖车过程很顺畅！
                </div>
              </div>
            </div>
          </el-col>
          <el-col :span="10" >
            <div class="car_story">
              <div class="car_story_img" style="background-position: 0 -800px" ></div>
              <div class="car_story_content">
                <div class="car_story_content_1">徐先生 | 建材商 | 宝马</div>
                <div class="car_story_content_2">
                  生意很忙没有多余时间去处理卖车的事情，车置宝从检测到卖车都是很方便，也不需要我去为价格操心，比我打算卖的的价格高了，很是意外，很开心。
                </div>
              </div>
            </div>
          </el-col>
        </el-row>
      <!--常见问答-->
      <el-row class="faq">
        <el-col class="faq_title">常见问答(FAQ)</el-col>
        <el-row>
        <el-col :span="7" :offset="4">
          <div class="faq_content">
            <div class="faq_content_1">Q1 兵丰远达怎么帮我买车？</div>
            <div class="faq_content_2">兵丰远达是专业汽车交易服务平台，每天有百万买家在这里选车，我们只将您的爱车卖给真实买家，在把您的爱车卖个公道价格的同时，完全杜绝了经销商、4S店对您的骚扰。</div>
          </div>
        </el-col>
        <el-col :span="7" :offset="2">
          <div class="faq_content">
            <div class="faq_content_1">Q2 通过兵丰远达出售车辆需要什么费用？</div>
            <div class="faq_content_2">我们不会向卖家收取任何费用，整个服务过程全部免费，在成交之后会向买家按车辆价款收取一定比例的服务费。兵丰远达承诺14天可退车，问题车辆退给兵丰远达售后。但兵丰远达明确收费的特殊卖车服务除外。</div>
          </div>
        </el-col>
        </el-row>
        <el-row>
        <el-col :span="7" :offset="4">
          <div class="faq_content">
            <div class="faq_content_1">Q3 卖车流程是什么？</div>
            <div class="faq_content_2">
              1、在此页面填写车辆信息，或拨打400-691-2670联系我们。<br>
              2、卖车顾问与您约定好时间地点后，评估师将上门对车辆进行初步评估，搜集车辆信息且对车辆进行拍照，评估师将依据兵丰远达大数据提供一个建议售价。<br>
              3、对于符合兵丰远达上架标准的车辆，兵丰远达将车辆信息及初步车况发布至兵丰远达平台，并予以多方推广，为您寻找买家。<br>
              4、带有购买意向的买家约见看车。<br>
              5、买家将与您签署《二手车买卖合同》，您须配合进行车辆复检，复检通过后方可办理车辆过户。
            </div>
          </div>
        </el-col>
        <el-col :span="7" :offset="2">
          <div class="faq_content">
            <div class="faq_content_1">Q4 在兵丰远达转让需要准备什么？</div>
            <div class="faq_content_2">
              需要先在网站提供您的联系电话，车辆品牌、型号等基本信息。待服务人员联系您后，在约定时间内准备好<br>
              1、身份证<br>
              2、行驶证<br>
              3、车辆登记证<br>
              4、车辆钥匙<br>
              5、车示标（环保标、检字标、交强险标）<br>
              6、交强险单<br>
              7、购置税本及购置税发票<br>
              8、购车发票/最近一次过户发票
            </div>
          </div>
        </el-col>
        </el-row>
        <el-row>
        <el-col :span="7" :offset="4">
          <div class="faq_content">
            <div class="faq_content_1">Q5 大概多长时间能够成交？</div>
            <div class="faq_content_2">兵丰远达是专业汽车交易服务平台，每天有百万买家在这里选车，我们只将您的爱车卖给真实买家，在把您的爱车卖个公道价格的同时，完全杜绝了经销商、4S店对您的骚扰。</div>
          </div>
        </el-col>
        </el-row>
      </el-row>
      <!--footer-->
      <home-footer></home-footer>
    </div>
</template>

<script>
import { HomeMenuBar, HomeFooter } from './common'

const imgArr = ['../static/images/001.jpg', '../static/images/002.jpg',
  '../static/images/003.jpg', '../static/images/004.jpg']

export default {
  name: 'Home',
  components: {
    HomeFooter,
    HomeMenuBar
  },
  data () {
    return {
      imgArr: imgArr
    }
  }
}
</script>

<style scoped>
  .el-carousel__item div {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 150px;
    margin: 0;
    width: 100%;
    height: 500px;
    background-position: center center;
    background-repeat: no-repeat;
    background-size: cover;
  }

  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }

  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }
  .compInfo{
    margin-top: 50px;
    height: 500px;
    background-image: url("../../static/images/005.jpg");
    background-position: center center;
    background-repeat: no-repeat;
    background-size: cover;
    color: #FFFFFF;
  }
  .compInfo .text1 {
    margin-top: 60px;
    font-weight: 400;
    font-size: 2.2rem;
  }
  .compInfo .text2 {
    margin-top: 10px;
    font-weight: 400;
    font-size: 1.6rem;
  }
  .gold_service{
    margin-top: 60px;
    height: 450px;
    background: linear-gradient(140deg,#FFEAAB 0,#E3BD6C 100%);
  }
  .gold_service h1{
    margin-top: 70px;
    margin-bottom: 80px;
    font-weight: 300;
    color: #8C5313;
  }
  .gold_service_content_1{
    position: relative;
    float: left;
  }
  .gold_service_content_2{
    position: relative;
    float: left;
    font-size: 1.2rem;
    color: #8C5313;
  }
  .gold_service_content_3{
    margin-top: 8px;
    position: relative;
    float: left;
    color: #8C5313;
    clear: both;
  }
  .gold_service_content_1 img{
    width: 40px;
  }
  .gold_service_content_box{
    margin-left: 20px;
    float: left;
  }
  .gold_service_space{
    background-color: #FFFFFF;
    height: 250px;
    padding-top: 90px;
    padding-left: 20px;
  }
  .car_story{
    position: relative;
   float: left;
    margin-top: 50px;
  }
  .car_story_img{
    position: relative;
    float: left;
    display: block;
    width: 136px;
    height: 136px;
    background: url(../../static/images/face.png) center no-repeat;
  }
  .car_story_content{
    position: relative;
    float: left;
    width: 14rem;
    margin-left: 5px;
  }
  .car_story_content_1{
    position: relative;
    float: left;
    font-weight: 500;
    font-size: 1.2rem;
  }
  .car_story_content_2{
    position: relative;
    float: left;
    width: 14rem;
    font-size: 0.9rem;
    margin-top: 8px;
    clear: both;
    text-align: left;
    line-height: 1.3rem;
  }
  .car_story_title{
    margin-top: 50px;
    font-size: 2.0rem;
    font-weight: 800;
  }
  .faq_content{
    text-align: left;
    margin-top: 50px;
  }
  .faq_content_1{
    font-size: 1.1rem;
    font-weight: 800;
    color: #333;
  }
  .faq_content_2{
    margin-top: 10px;
    font-size: 0.9rem;
    font-weight: 400;
    color: #999;
    line-height: 1.45rem;
  }
  .faq_title{
    margin-top: 80px;
    font-size: 1.8rem;
    font-weight: 600;
   }
  .faq{
    background-color: aliceblue;
    margin-top: 80px;
    padding-bottom: 50px;
  }
</style>
