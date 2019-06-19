<template>
  <div class="shouhou">
    <img src="../../../static/images/tu1.jpg" alt>

    <div class="bottom1">
      <Row style="margin-bottom:4%">
        <Col span="6">
          <Card class="card" shadow>
            <p
              style="font-size:30px;
font-family:PingFang-SC-Bold;
font-weight:bold;
color:rgba(38,32,34,1);margin-bottom:20px;"
            >在线交谈</p>
          <span  style="display:block;font-size:18px;
font-family:PingFang-SC-Regular;
font-weight:400;
color:rgba(83,83,83,1);
margin-bottom:58px">
            
                            工作日 9:00-12:00 14:00-18:00
客服代表一对一即时消息沟通
                        
          </span>
            <!-- <Button style="background:#1D2088;color:#f6f6f6;margin-top:15%;" >售前在线咨询</Button> -->

            <Button class="btn1" style="color:#262022;margin-top:5%;border:1px solid #262022; border-radius: 0"><span class="span1">立即在线交谈
              </span> </Button>
          </Card>
        </Col>
        <Col span="6">
        <Card class="card" shadow>
            <p
              style="font-size:30px;
font-family:PingFang-SC-Bold;
font-weight:bold;
color:rgba(38,32,34,1);margin-bottom:20px;"
            >项目咨询</p>
          <span  style="display:block;font-size:18px;
font-family:PingFang-SC-Regular;
font-weight:400;
color:rgba(83,83,83,1);
margin-bottom:58px">
            
                        
                            免费一对一项目与解决方案咨询服务
1个工作日内为您安排资深销售顾问
                        
                        
          </span>
            <!-- <Button style="background:#1D2088;color:#f6f6f6;margin-top:15%;" >售前在线咨询</Button> -->

            <Button class="btn1" style="color:#262022;margin-top:5%;border:1px solid #262022; border-radius: 0"><span class="span1">填写咨询表单
              </span> </Button>
          </Card>
        </Col>
        <Col span="6">
            <Card class="card" shadow>
            <p
              style="font-size:30px;
font-family:PingFang-SC-Bold;
font-weight:bold;
color:rgba(38,32,34,1);margin-bottom:20px;"
            >电话咨询</p>
          <span  style="display:block;
          width:288px;font-size:18px;
font-family:PingFang-SC-Regular;
font-weight:400;
color:rgba(83,83,83,1);
margin-bottom:32px">
全国统一售前服务热线，若遇线路繁忙，请选择 在线交谈 进行产品和服务咨询
                        
                        
                        
          </span>
            <!-- <Button style="background:#1D2088;color:#f6f6f6;margin-top:15%;" >售前在线咨询</Button> -->

            <Button class="btn1" style="color:#262022;margin-top:5%;border:1px solid #262022; border-radius: 0"><span class="span1">填写咨询表单
              </span> </Button>
          </Card>
          <!-- <Card class="card" shadow>
            <p
              style="font-family:PingFang-SC-Bold;font-size:30px;color:#172A88;text-align:center;margin-bottom:20px;"
            >电话咨询</p>
            <p
              style="color:#535353;font-size:18px; font-family:PingFang-SC-Regular;line-height:25px "
            >全国统一售前服务热线，若遇线路繁忙，请选择 在线交谈 进行产品和服务咨询</p>
            <p
              style="color:#172A88;font-size:30px;margin-top:16%;font-weight:400;font-family:Impact;"
            >021-2281-9090</p>
          </Card> -->
        </Col>
      </Row>
      <Row style="margin-top:50px;">
        <Col span="9" style="margin-right:90px">
          <Card class="card1" shadow>
            <p
              style="font-size:30px;
font-family:PingFang-SC-Medium;
font-weight:500;
color:rgba(38,32,34,1);margin-bottom:20px;text-align:center;"
            >成为销售合作伙伴</p>
            <p
              style="color:#535353;font-size:18px; font-family:PingFang-SC-Regular;line-height:25px; "
            >越梧渠道化市场战略以及全方位的渠道体系支持,期待与您携手</p>
             <Button class="btn1" style="color:#262022;margin-top:5%;border:1px solid #262022; border-radius: 0"><span class="span1">立即申请
              </span> </Button>
            <!-- <Button style="background:#1D2088;color:#f6f6f6;margin-top:15%;" >立即申请</Button> -->
          </Card>
        </Col>
        <Col span="9">
          <Card class="card1" shadow>
            <p
              style="font-size:30px;
font-family:PingFang-SC-Medium;
font-weight:500;
color:rgba(38,32,34,1);margin-bottom:20px;text-align:center;"
            >成为销售合作伙伴</p>
            <p
              style="color:#535353;font-size:18px; font-family:PingFang-SC-Regular;line-height:25px; "
            >致力于建设高效、互利共赢的供应商协作体系，与您共谋行业发展</p>
             <Button class="btn1" style="color:#262022;margin-top:5%;border:1px solid #262022; border-radius: 0"><span class="span1">立即申请
              </span> </Button>
            <!-- <Button style="background:#1D2088;color:#f6f6f6;margin-top:15%;" >立即申请</Button> -->
          </Card>
        </Col>
      </Row>
    </div>
    
  </div>
</template>
<script>
export default {
  name: "shouhou",
  data() {
    return {};
  },
  mounted() {}
};
</script>
<style lang="scss" scoped>
.shouhou {
  padding-top: 4%;
  // width: 200px;
  height: 100%;
  background: #f6f6f6;
  text-align: center;
  .btn {
    &:hover {
     
      color: red;
      // background:#1D2088;
    }
  }
  img {
    width: 100%;
    margin-bottom: 60px;
  }
  span {
    font-family: "PingFang-SC-Medium";
    font-size: 40px;
    color: #12277f;
  }

  .bottom1 {
    text-align: left;
    margin: 0 auto;
    margin-top: 24px;
    // width: 74.0625rem;
    // height: 1018px;
    background: #f6f6f6;
    padding-left: 383px;
    padding-bottom: 160px;
    .ivu-col-span-6 {
      width: 27%;
    }
    .card {
      // margin-right: 48px;
      height: 292px;
      width: 354px;
      // margin-right: 15%;
      .btn1{
        .span1{
font-size:18px;
font-family:PingFang-SC-Regular;
font-weight:400;
color:rgba(38,32,34,1);
        }
        // background: red;
        &:hover {
          background: #262022;
              .span1{

                color: #f6f6f6;
              }        
        }
      }
    }
    .card1 {
      // margin-right: 50px;
        margin-left: -50px;
      height: 221px;
      width: 602px;
       .btn1{
        .span1{
font-size:18px;
font-family:PingFang-SC-Regular;
font-weight:400;
color:rgba(38,32,34,1);
        }
        // background: red;
        &:hover {
          background: #262022;
              .span1{

                color: #f6f6f6;
              }        
        }
      }
    }
  }
}
</style>

