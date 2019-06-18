<template>
  <div class="design">
    <Card class="card" shadow>
      <p class="header">时代背景</p>

      <p class="content">十八大以来，党中央高度重视意识形态领域工作，党建宣传的需求。</p>
      <br>
      <p class="content">改革开放40周年以来建设的成就的宣传，增强凝聚力。</p>
    </Card>
    <Card class="card1" shadow>
      <p class="header">展厅现状</p>
      <div class="xian"></div>
      <div class="triangle_border_down">
        <span></span>
      </div>

      <Row :gutter="16">
        <Col span="6">
          <img src="../../../static/images/图层 1.png" alt>
          <span class="content1">展示单一</span>
          <span class="content2">
            展示形式单一
            <br>主要采用灯箱图文形式
          </span>
        </Col>
        <Col span="6">
          <img src="../../../static/images/图层 2.png" alt>
          <span class="content1">较大空间</span>
          <span class="content2">
            展示内容众多
            <br>需要较大的展示空间
          </span>
        </Col>
        <Col span="6">
          <img src="../../../static/images/图层 3.png" alt>
          <span class="content1">&nbsp;&nbsp;&nbsp;缺乏灵活性</span>
          <span class="content2">
            针对不同类型的参观群体
            <br>讲解服务缺乏灵活性
          </span>
        </Col>
        <Col span="6">
          <img src="../../../static/images/图层 4.png" alt>
          <span class="content1">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; 响应速度欠缺</span>
          <span class="content2">
            展示形式单一
            <br>主要采用灯箱图文形式
          </span>
        </Col>
      </Row>
    </Card>
    <div class="card2">
      <div class="triangle_border_left">
        <span></span>
      </div>
      <span class="content">越梧优势：</span>
    </div>
    <Row style="width:1136px;padding:20px;margin:0 auto;">
      <Col span="11">
        <div class="youshi">
          <img class="tupian" src="../../../static/images/图层 5.png" alt>
          <div class="youshi_r">
            <span>参观人员</span>
            <p>沉浸感：环境营造</p>
            <p>多样性：不同类型的参观者看到不同的内容</p>
            <p>个性化：参观过程中能够随需应变</p>
          </div>
        </div>
      </Col>
      <Col span="11" offset="2">
        <div class="youshi">
          <img class="tupian" src="../../../static/images/图层 6.png" alt>
          <div class="youshi_r">
            <span>建设方</span>

            <p>省成本：减少硬件投入</p>
            <p>省空间：节约场地</p>
            <p>省人员：减少操作人员及讲解人员</p>
          </div>
        </div>
      </Col>
    </Row>
    <Row style="width:1136px;padding:20px;margin:0 auto;margin-top:2%">
      <Col span="11">
        <div class="youshi">
          <img class="tupian" src="../../../static/images/图层 7.png" alt>
          <div class="youshi_r">
            <span>讲解人员</span>

            <p>个性讲解：根据每场参观者不同的需求，提前定制讲解词。</p>
            <p>智能展示：参观过程中，随机应变，随需应变调度展示内容。</p>
            <p>讲解辅助：降低讲解词记忆难度，讲解现场获取讲解提示。</p>
          </div>
        </div>
      </Col>
      <Col span="11" offset="2">
        <div class="youshi">
          <img class="tupian" src="../../../static/images/图层 8.png" alt>
          <div class="youshi_r">
            <span>操作维护人员</span>

            <p>资源管理：全馆设备、媒体内容统一管理。</p>
            <p>场景配置：针对客户类型，全馆演示内容整体配置。</p>
            <p>便捷操作：设备操作控制信息化。操作指令任意组合，设备控制一键操作。</p>
            <p>智能管理：设置各类是被告警阈值，告警方式，统一监控场馆设备运行。故障预警。</p>
          </div>
        </div>
      </Col>
    </Row>
       <div class="card2">
      <div class="triangle_border_left">
        <span></span>
      </div>
      <span class="content" >设计理念：</span>
      <p>
          
                            带给参观者自由的空间，艺术的享受，人文的关怀。在愉悦的氛围下，理解办展者的所要传达的思想，并形成共鸣。<br>
科技与艺术相结合。以艺术为表现形式，以科技为实现手段。将最新的物联网技术为感知手段；以人工智能和大数据分析为控制中枢；
以新颖的媒体展现形式为输出。实现舒适的参观环境、自由的空间延展、快速的内容调度、炫目的展示效果。<br>
我们拥有科学严谨的管理体系和成熟的实施团队来应对各种挑战，确保项目高效有序地运行。<br>
对项目的整个过程进行严格监控，确保项目实施中的每一个环节都在科学、权威的管理体系之下。最终实现设计效果与实体效果的高度一致。
                        
      </p>
    </div>
  </div>
</template>
<script>
export default {
  name: "design",
  data() {
    return {};
  },
  mounted() {}
};
</script>
<style lang="scss" scoped>
.design {
  height: 1720px;
  width: 100%;
  background: url("../../../static/images/设计理念.jpg") no-repeat;
  .card {
    top: 7%;
    width: 1440px;
    height: 205px;
    background: #ffffff;
    margin: 0 auto;
    text-align: center;
    .header {
      font-size: 30px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(41, 41, 41, 1);
      margin-bottom: 2%;
    }
    .content {
      font-size: 18px;
      font-family: PingFang-SC-Regular;
      font-weight: 400;
      color: rgba(41, 41, 41, 1);
    }
  }
  .card1 {
    top: 10%;
    width: 1440px;
    height: 412px;
    background: #ffffff;
    margin: 0 auto;
    text-align: center;
    padding-top: 1%;
    margin-bottom: 15%;
    .header {
      font-size: 30px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(41, 41, 41, 1);
      margin-bottom: 0%;
    }
    .content {
      font-size: 18px;
      font-family: PingFang-SC-Regular;
      font-weight: 400;
      color: rgba(41, 41, 41, 1);
    }
    .xian {
      width: 160px;
      height: 2px;
      background: #facc09;
      margin: 0 auto;
    }
    .content1 {
      margin-top: 6%;
      margin-bottom: 6%;
      display: block;
      font-size: 24px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(41, 41, 41, 1);
    }
    .content2 {
      font-size: 16px;
      font-family: PingFang-SC-Regular;
      font-weight: 400;
      color: rgba(41, 41, 41, 1);
      line-height: 24px;
      margin-left: 36%;
      display: block;
      text-align: left;
    }
    .triangle_border_down span {
      display: block;
      width: 0;
      height: 0;
      border-width: 12px 12px 0;
      border-style: solid;
      border-color: #facc09 transparent transparent; /*黄 透明 透明 */
      margin: 0 auto;
      margin-bottom: 3%;
    }
  }
  .card2 {
    height: 40px;
    width: 100%;
    .content {
      font-size: 30px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(41, 41, 41, 1);
    }
    .triangle_border_left span {
      display: block;
      width: 0;
      height: 0;
      border-width: 15px 15px 15px 0;
      border-style: solid;
      border-color: transparent #facc09 transparent transparent; /*透明 黄 透明 透明 */
      margin-left: 307px;
      margin-right: 1%;
      float: left;
      margin-top: 0.5%;
    }
    p{
        display: block;
        padding-top: 2%;
        padding-left: 2.3%;
        width: 1160px;
        margin: 0 auto;
        font-size:18px;
        font-family:PingFang-SC-Medium;
        font-weight:500;
        color:rgba(41,41,41,1);
    }
  }
  .youshi {
    height: 110px;
    .tupian {
      display: block;
      padding-top: 5%;
      padding-left: 10%;
      float: left;
    }
    .youshi_r {
      padding-top: 5%;
      padding-left: 5%;
      width: 400px;
      float: left;
      span {
        font-size: 18px;
        font-family: PingFang-SC-Medium;
        font-weight: 500;
        color: rgba(41, 41, 41, 1);
      }
      p {
        font-size: 16px;
        font-family: PingFang-SC-Regular;
        color: rgba(41, 41, 41, 1);
        margin-bottom: 1%;
        &:nth-child(2) {
          margin-top: 5%;
        }
      }
    }
  }
}
</style>

