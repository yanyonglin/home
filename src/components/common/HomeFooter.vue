<template>
  <div class="footer_top">
    <el-row>
      <el-col class="footer_icon" :span="4" :offset="2">
        <div>
          <span class="footer_icon_img"><img src="../../../static/images/f01.png" alt="" /></span>
          <span class="footer_icon_text">一年/两万公里质保</span>
        </div>
      </el-col>
      <el-col class="footer_icon" :span="4">
        <div>
          <span class="footer_icon_img"><img src="../../../static/images/f02.png" alt="" /></span>
          <span class="footer_icon_text">14天可退</span>
        </div>
      </el-col>
      <el-col class="footer_icon" :span="4">
        <div>
          <span class="footer_icon_img"><img src="../../../static/images/f03.png" alt="" /></span>
          <span class="footer_icon_text">249项检测</span>
        </div>
      </el-col>
      <el-col class="footer_icon" :span="4">
        <div>
          <span class="footer_icon_img"><img src="../../../static/images/f04.png" alt="" /></span>
          <span class="footer_icon_text">精选优质车源</span>
        </div>
      </el-col>
      <el-col class="footer_icon" :span="4">
        <div>
          <span class="footer_icon_img"><img src="../../../static/images/f05.png" alt="" /></span>
          <span class="footer_icon_text">一站式服务</span>
        </div>
      </el-col>
    </el-row>
    <el-row class="footer_href_top">
      <el-col :span="5" :offset="2">
        <el-row class="footer_href_title"><el-col :pull="6">关于我们</el-col></el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">公司介绍</el-col>
          <el-col :span="8" >服务条款</el-col>
        </el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">联系我们</el-col>
          <el-col :span="8" >隐私政策</el-col>
        </el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">加入我们</el-col>
          <el-col :span="8" >法律申明</el-col>
        </el-row>
      </el-col>
      <el-col :span="4" >
        <el-row class="footer_href_title"><el-col :pull="6">交易流程</el-col></el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">买车流程</el-col>
        </el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">异地购车</el-col>
        </el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">运费规则</el-col>
        </el-row>
      </el-col>
      <el-col :span="5" :pull="1">
        <el-row class="footer_href_title"><el-col :pull="6">新车精选</el-col></el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">新车资讯</el-col>
          <el-col :span="8" >贷款资讯</el-col>
        </el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">购车问答</el-col>
          <el-col :span="8" >补贴购车</el-col>
        </el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">车型估价</el-col>
        </el-row>
      </el-col>
      <el-col :span="5" >
        <el-row class="footer_href_title"><el-col :pull="0">400-888-8888</el-col></el-row>
        <el-row class="footer_href_title">
          <el-col :span="20" :offset="2">周一至周日 0:00-24:00</el-col>
        </el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">在线资讯</el-col>
          <el-col :span="8" >投诉建议</el-col>
        </el-row>
        <el-row class="footer_href_content">
          <el-col :span="8" :offset="2">举报违规</el-col>
        </el-row>
      </el-col>
    </el-row>
    <!--备案号-->
    <el-row class="footer_copy_info">
      <el-col>北京兵丰远达汽车贸易有限公司&copy;2003-2018</el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'HomeFooter'
}
</script>

<style scoped>
.footer_top{
  background-color: #4C4C4C;
  color: #FFF;
  padding-top: 30px;
}
.footer_icon_img img{
  display: block;
  float: left;
  width: 32px;
  padding-top: 5px;
}
.footer_icon_text{
  display: block;
  float: left;
 margin-top: 10px;
}
.footer_href_top{
  margin-top: 20px;
  line-height: 1.2rem;
  padding-bottom: 50px;
}
.footer_href_title{
  margin-top: 10px;
  font-size: 1.1rem;
}
.footer_href_content{
 margin-top: 10px;
  line-height: 1.1rem;
  color: #A2A2A2;
}
.footer_copy_info{
  padding-bottom: 20px;
  color: gray;
}
</style>
