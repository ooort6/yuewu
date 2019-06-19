<template>
  <div class="home">
    <div class="banner">
      <Carousel
        autoplay
        :autoplay-speed="6000"
        arrow="always"
        trigger="hover"
        loop
        radius-dot
        easing
      >
        <CarouselItem>
          <div class="demo-carousel">
            <img src="@/static/images/轮播.jpg" alt>
          </div>
        </CarouselItem>
        <CarouselItem>
          <div class="demo-carousel">
            <img src="@/static/images/轮播2.jpg" alt>
          </div>
        </CarouselItem>
      </Carousel>
    </div>
    <!--轮播 -->
    <!-- 主体 -->
    <div class="index-container">
      <!-- one -->
      <div class="index-phone-center">
        <div class="section-box section-phone-box">
          <div class="section-title" style="margin-top:-40px"></div>
          <div class="section-box-adv" style="background:#fff">
            <Row :gutter="16" style="width:1200px;margin:0 auto;margin-top:2%">
              <Col span="8">
                <Card :dis-hover="true" :bordered="false" style="height:298px;padding-top:30px; ">
                  <div
                    style="text-align:center;position:relative"
                  >
                    <!-- <img src="@/static/image/微信图片_20190604151034.png" style="position:absolute;top:40%; color:#00366F;font-size:24px; left:32%" alt="">
                    <img src="@/static/image/1.png">
                    <br>
                    <span class="adv-font">查看详情</span>
                    <span class="adv-img"></span>-->
                    <img src="../../static/images/目标.png" alt>
                    <br>
                    <span class="adv-font">目标</span>
                    <br>
                    <span class="adv-font-bottom">
                      带给参观者自由空间
                      <br>艺术享受，人文关怀
                      <br>理解办展者思想，形成共鸣
                    </span>
                  </div>
                </Card>
              </Col>
              <Col span="8">
                <Card :dis-hover="true" :bordered="false" style="height:298px;padding-top:30px; ">
                  <div
                    style="text-align:center;position:relative"
                  >
                    <!-- <img src="@/static/image/微信图片_20190604151034.png" style="position:absolute;top:40%; color:#00366F;font-size:24px; left:32%" alt="">
                    <img src="@/static/image/1.png">
                    <br>
                    <span class="adv-font">查看详情</span>
                    <span class="adv-img"></span>-->
                    <img src="../../static/images/方法.png" alt>
                    <br>
                    <span class="adv-font">方法</span>
                    <br>
                    <span class="adv-font-bottom">
                      科技与艺术相结合
                      <br>以艺术为表现形式
                      <br>以科技为实现手段
                    </span>
                  </div>
                </Card>
              </Col>
              <Col span="8">
                <Card :dis-hover="true" :bordered="false" style="height:298px;padding-top:30px; ">
                  <div
                    style="text-align:center;position:relative"
                  >
                    <!-- <img src="@/static/image/微信图片_20190604151034.png" style="position:absolute;top:40%; color:#00366F;font-size:24px; left:32%" alt="">
                    <img src="@/static/image/1.png">
                    <br>
                    <span class="adv-font">查看详情</span>
                    <span class="adv-img"></span>-->
                    <img src="../../static/images/实现.png" alt>
                    <br>
                    <span class="adv-font">实现</span>
                    <br>
                    <span class="adv-font-bottom">
                      应对各种挑战
                      <br>最终实现设计效果
                      <br>与实体效果的高度一致
                    </span>
                  </div>
                </Card>
              </Col>
            </Row>
          </div>
        </div>
      </div>
      <div style="width:100%;height:200px;margin-top:50px;margin-bottom:200px">
        <img src="../../static/images/图2.png" alt style="width:100%;height:300px">
      </div>

      <div class="case">
        <Row :gutter="16" justify="space-around" class="card" style="padding:20px;border:none">
          <i-col class="i-col" span="5" offset="4" style="margin-right:18px">
            <div @click="$router.push({name: 'control', params: { ins:0}})">
              <!-- <img src="../../static/images/1.00.png" alt=""> -->
              <Card shadow>
                <img src="../../static/images/1.00.png" alt>
                <div class="mask"></div>
                <img class="inimg" src="../../static/images/智慧展厅控制系统 .png" alt>
                <i class="inimg_r"></i>
              </Card>
            </div>
          </i-col>
          <i-col class="i-col" span="5" offset="1" style="margin-right:18px">
            <div @click="$router.push({name: 'control', params: { ins:1}})">
              <Card shadow>
                <img src="../../static/images/2.00.png" alt>
                <div class="mask"></div>
                <img class="inimg" src="../../static/images/高精度定位系统.png" alt>
                <i class="inimg_r"></i>
              </Card>
            </div>
          </i-col>
          <i-col class="i-col" span="5" offset="1" style="margin-right:18px;margin-bottom:2%">
            <div @click="$router.push({name: 'control', params: { ins:2}})">
              <Card shadow>
                <img src="../../static/images/3.00.png" alt>
                <div class="mask"></div>
                <img class="inimg" src="../../static/images/智能视频分析系统.png" alt>
                <i class="inimg_r"></i>
              </Card>
            </div>
          </i-col>

          <i-col class="i-col" span="5" offset="7" style="margin-right:18px">
            <div @click="$router.push({name: 'control', params: { ins:3}})">
              <Card shadow>
                <img src="../../static/images/4.00.png" alt>
                <div class="mask"></div>
                <!-- <span class="inimg">智慧展厅控制系统</span> -->
                <img class="inimg" src="../../static/images/虚拟巡游系统 .png" alt>
                <i class="inimg_r"></i>
              </Card>
            </div>
          </i-col>
          <i-col class="i-col" span="5" offset="1" style="margin-right:18px">
            <div @click="$router.push({name: 'control', params: { ins:4}})">
              <Card shadow>
                <img src="../../static/images/5.00.png" alt>
                <div class="mask"></div>
                <img class="inimg" src="../../static/images/自助导览系统.png" alt>
                <i class="inimg_r"></i>
              </Card>
            </div>
          </i-col>
        </Row>
      </div>

      <div class="partner">
        <header>
          <span class="partner_1">成功案例</span>
          <br>
          <span class="partner_2">Successful cases</span>
          <div class="partner_3">
            <div class="partner_4"></div>
          </div>
        </header>
        <div class="partner-content">
          <div class="partner_5"></div>
          <img src="../../static/images/6.00.png" alt>
          <img src="../../static/images/6.00.png" alt>
          <img src="../../static/images/6.00.png" alt>
          <div class="partner_6"></div>
        </div>
        <div class="partner-bottom">
          <div class="partner_7"></div>
        </div>
      </div>
      <div class="aboutUs">
       <header>
          <span class="partner_1">关于我们</span>
          <br>
          <span class="partner_2">About Us</span>
          <div class="partner_3">
            <div class="partner_4"></div>
          </div>
        </header>
        <content>
         <p>
           
   上海越梧信息科技有限公司有一家聚焦于展览展示创意设计及技术研发的高科技公司。公司首创“艺术创造美好，科技服务生活，实现合作共赢”经营理念，以智慧展示系统为核心，跨界融合策划创意、空间装饰、互动科技、软件开发、数字CG、影视制作、系统集成、舞美灯光、平面设计、建筑模型等行业，打造中国展览展示行业全新产业链模式。公司现有员工50多人，其中研发及设计人员占比超过80%。公司以人工智能技术为核心，以各种高科技数字化展示技术手段如：全息投影、VR、AR、大数据可视化等为辅助，完成了诸多展示场馆及临展的设计及实施工作。客户范围跨越政府、电信运营商、大型制造企业、电力、能源等多个行业。
                        
         </p>

          <!-- <pre>上海智天信息科技有限公司成立于2012年。2015年通过工信部软件企业评审。公司业务主要集中于安全领域，拥有完整地安全产品线。经过近10年的发展，公司业务范围不断扩大，业界知名度不断提升。目前，公司客户群体主要集中在政府、事业单位以及大型企业。</pre>
            <pre>在信息系统安全防护方面，提供网络层的恶意代码防护系统，采用领先的DGA以及智能学习算法，使APT检测能力达到业界领先水平。防止企业信息系统被植入木马病毒而成为黑客不法工具，或者机密信息被窃取等。</pre>
            <pre>在业务安全方面，提供网络内容审核系统，采用智天自有的文本快速匹配算法以及图形分析算法，实现文本、图片以及视频内容审核。防止内部人员滥用网络，对外发送敏感文件或不良内容。</pre>
          <pre>在企业运营安全管理方面，提供安全管理平台，对人、物、环境进行全方位安全管理。引入人工智能技术，实现事前预警，事中记录，事后分析形成新的智能判断规则的持续优化能力。</pre>-->
        </content>
      </div>
      <!-- 智能配件 -->
      <!-- <div class="box-img-black"></div> -->

      <!-- 生活周边 -->
    </div>

    <!-- <BackTop :height="400" :right="0" :bottom="648" >
        <div class="top"
      
        
        >
            <img
        src="../../static/image/TOP.png"
        style=" position: absolute;top: 50%;left: 50%;transform: translate(-50%, -50%);"
        alt
      >
        </div>
    </BackTop>
    
    <BackTop :height="400" :right="0" :bottom="593" >
        <div class="top"
        >
            <img
        src="../../static/image/TOP.png"
        style=" position: absolute;top: 50%;left: 50%;transform: translate(-50%, -50%);"
        alt
      >
        </div>
    </BackTop>-->
  </div>
</template>
<script>
import { mapState, mapGetters, mapActions } from "vuex";
export default {
  name: "home",
  data() {
    return {
      num: 5,
      isnode: false
    };
  },
  mounted() {
    if (1) {
      this.$store.dispatch("footerStatus/getNewNum", this.num);
      // console.log(this.num)
      this.$store.dispatch("footerStatus/hideFooter");
    } else {
      this.$store.dispatch("footerStatus/showFooter");
    }
    // console.log(this.a);
    // console.log(this.$store.state.showFooter)
  },
  computed: {
    //  ...mapState({  //这里的...是超引用，ES6的语法，意思是state里有多少属性值我可以在这里放多少属性值
    //        isShow:state=>state.footerStatus.showFooter //注意这些与上面的区别就是state.footerStatus,
    //                                                     //里面定义的showFooter是指footerStatus.js里state的showFooter
    //     }),
    ...mapGetters("footerStatus", {
      //footerStatus指的是modules文件夹下的footerStatus.js模块
      isShow: "isShow", //第一个isShow是我自定义的只要对应template里v-if="isShow"就行，
      a: "getChangedNum" //第二个isShow是对应的footerStatus.js里的getters里的isShow
    })
  },
  watch: {},
  methods: {
    // phoneDetails(item){
    // 	this.$router.push({name:'details', query:{main_id:item.main_id}})
    // },
    // headsetDetails(item){
    // 	this.$router.push({name:'details', query:{main_id:item.main_id}})
    // },
    // partDeatils(item){
    // 	this.$router.push({name:'details', query:{main_id:item.main_id}})
    // },
    // arroundDetails(item){
    // 	this.$router.push({name:'details', query:{main_id:item.main_id}})
    // },
    // async _getphonelist(){ // 手机
    // 	const res = await getphonelist()
    // 	if(res.status == 0){
    // 		this.phonelist = res.result
    // 	}
    // },
    // async _getheadsetList(){ // 声学
    // 	const res = await getheadsetlist()
    // 	if(res.status == 0){
    // 		this.headsetlist = res.result
    // 	}
    // },
    // async _getpartlist(){ // 配件
    // 	const res = await getpartlist()
    // 	if(res.status == 0){
    // 		this.partlist = res.result
    // 	}
    // },
    // async _getarroundlist(){ // 生活周边
    // 	const res = await getarroundlist()
    // 	if(res.status == 0){
    // 		this.arroundlist = res.result
    // 	}
    // },
  }
};
</script>
<style lang="scss" scoped>
.ivu-carousel > .ivu-carousel-arrow {
  background-color: #fff;
}
.home {
  padding-top: 4%;
  background: #fff;
  .banner {
    width: 100%;
    // height: 800px;
    img {
      display: block;
      width: 100%;
      height: 800px;
    }
  }
  .index-adv-center {
    margin-bottom: 50px;
  }
  .ivu-card {
    // position: relative;
    // overflow: hidden;
    img {
      // width: 100%;
      // height: 100%;
      // display: block;
      // transition: all 2s;
      // position: absolute;
      // top: 63px;
      // left: 95px;
    }
    :hover {
      // width: 80%;
      // height: 80%;
    }
  }

  .section-box {
    margin-bottom: 0px;
    .box-img {
      display: block;
      width: 100%;
      height: 100%;
      text-align: center;
      background-repeat: no-repeat;
      background-position: center;
    }

    a {
      position: relative;
    }
    .section-title {
      padding-top: 20px;

      font-size: 30px;
      text-align: center;
      margin-bottom: 10px;
      h3 {
        margin-bottom: 8px;
      }
      p {
        text-align: center;
        font-size: 16px;
        color: #888;
        margin-bottom: 18px;
      }
    }

    .section-box-adv {
      height: 380px;
      padding-bottom: 45px;
      background-color: #fff;
      border-bottom: 1px solid #fff;
      overflow: hidden;
      .ivu-card {
      }
      // .ivu-card {
      //   position: relative;
      //   &:hover {
      //     cursor: pointer;
      //     opacity: 0.9;
      //     position: relative;
      //     animation: mymove 1s linear 0s infinite alternate;
      //     -webkit-animation: mymove 1s linear 0s infinite alternate;
      //   }
      //   @keyframes mymove {
      //     from {
      //       bottom: 0px;
      //     }
      //     to {
      //       bottom: 20px;
      //     }
      //   }

      //   @-webkit-keyframes mymove /*Safari and Chrome*/ {
      //     from {
      //       bottom: 0px;
      //     }
      //     to {
      //       bottom: 20px;
      //     }
      //   }
      // }
      .adv-font {
        width: 68px;
        height: 34px;
        font-size: 36px;
        font-family: PingFang-SC-Medium;
        font-weight: 500;
        color: rgba(41, 41, 41, 1);
        // cursor: pointer;
      }
      .adv-font-bottom {
        display: block;
        text-align: left;
        margin-top: 5%;
        margin-left: 38%;
        width: 224px;
        height: 81px;
        font-size: 18px;
        font-family: PingFang-SC-Regular;
        font-weight: 400;
        color: rgba(41, 41, 41, 1);
        // cursor: pointer;
      }
      .adv-img {
        width: 21.5px;
        height: 21.5px;
        display: block;
        float: right;
        margin-right: 10%;
        margin-top: 3%;
        background: url("../../static/image/查看详情.png");
        cursor: pointer;
      }
      p {
        text-align: left;
        margin-left: 120px;
        font-size: 14px;
        color: #888;
        margin-bottom: 18px;
      }
      i {
        display: block;
        text-align: center;
        font-size: 14px;
        color: #888;
        margin-bottom: 18px;
      }
      h2 {
        font-size: 18px;
        margin: 18px;
        color: #20273c;
        margin-bottom: 8px;
      }
      .box-img {
        width: 100%;
      }
      ul {
        overflow: hidden;
        width: 1240px;
        margin: auto;
        li {
          text-align: center;
          float: left;
          position: relative;
          width: 25%;
          padding-top: 45px;
          .box-img {
            display: block;
            width: 100%;
            height: 100%;
            text-align: center;
            background-repeat: no-repeat;
            background-position: center;
          }
          .phone_wraper {
            position: relative;
            img {
              height: 130px;
              &:hover {
                cursor: pointer;
                opacity: 0.9;
                position: relative;
                animation: mymove 1s linear 0s infinite alternate;
                -webkit-animation: mymove 1s linear 0s infinite alternate;
              }
              @keyframes mymove {
                from {
                  bottom: 0px;
                }
                to {
                  bottom: 20px;
                }
              }

              @-webkit-keyframes mymove /*Safari and Chrome*/ {
                from {
                  bottom: 0px;
                }
                to {
                  bottom: 20px;
                }
              }
            }

            em {
              font-style: normal;
              display: block;
              color: #333;
              font-size: 20px;
            }
            p {
              font-size: 14px;
              color: #999;
            }
          }
        }
        .last {
          margin-right: 0;
        }
      }
    }
  }

  .case {
    width: 100%;
    height: 600px;
    // padding-top: -15px;
    margin-bottom: 6%;
    .i-col {
      width: 350px;
      height: 270px;
      text-align: center;
      font-family: "PingFang-SC-Medium";
      font-size: 24px;
      color: #003672;
      border-bottom: none;
      // cursor: pointer;
    }
    .ivu-card-shadow {
      box-shadow: none;
    }
    img {
      position: relative;
    }
    .mask {
      position: absolute;
      top: 5.8%;
      left: 6%;
      width: 365px;
      height: 231px;
      border-radius: 8%;
      background: rgba(153, 223, 255, 0.3);
      color: #ffffff;
      opacity: 0;
      &:hover {
        opacity: 1;
      }
    }
    .inimg {
      position: absolute;
      bottom: 15%;
      left: 15%;
      color: #facc09;
      font-size: 18px;
      cursor: pointer;
    }
    .inimg_r {
      width: 31px;
      height: 31px;
      position: absolute;
      bottom: 15%;
      right: -5%;
      //  background: url('../../static/images/点击 (1).0.png') no-repeat;

      background: url("../../static/images/点击 (1).png") no-repeat;
      &:hover {
        background: url("../../static/images/点击 (1).0.png") no-repeat;
      }
    }
  }

  .partner {
    width: 100%;
    height: 520px;
    padding-top: 43px;
    background: #f6f6f6;
    margin: 0 auto;
    .partner-content {
      width: 1167px;
      height: 222px;
      // background: red;
      margin: 0 auto;
      .partner_5 {
        width: 82px;
        height: 100%;
        border: 2px solid rgba(105, 105, 105, 0.2);
        border-right: none;
        float: left;
      }
      .partner_6 {
        width: 82px;
        height: 100%;
        border: 2px solid rgba(105, 105, 105, 0.2);
        border-left: none;
        float: right;
      }
      img {

        margin-top: 2%;
        margin-left: 2%;

        margin-right: 4%;
        transition: transform 0.5s;
        &:hover{
          transform: translate(0,-10px);
          cursor: pointer;
        //           position: relative;
        // animation: mymove 0.5s infinite;
        // -webkit-animation: mymove 0.5s infinite; /*Safari and Chrome*/
        }
      }
      // @keyframes mymove {
      //   from {
      //     top: 0px;
      //   }
      //   to {
      //     top: -15px;
      //   }
      // }

      // @-webkit-keyframes mymove /*Safari and Chrome*/ {
      //   from {
      //     top: 0px;
      //   }
      //   to {
      //     top: -15px;
      //   }
      // }

      img:nth-child(4) {
        margin-top: 2%;
        margin-right: 0;
      }
    }
    .partner-bottom{
       width: 372px;
      height: 6px;
      background: #facc09;
      margin: 0 auto;
      margin-top: 35px;
      .partner_7{
        width: 108px;
      height: 6px;
      background: #262022;
      margin: 0 auto;
      }
    }
  }

  .partner header {
    width: 100%;
    height: auto;
    margin: 0 0 58px 0;
    text-align: center;
    .partner_1 {
      width: 145px;
      height: 34px;
      font-size: 36px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(41, 41, 41, 1);
    }
    .partner_2 {
      width: 140px;
      height: 13px;
      font-size: 16px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(41, 41, 41, 1);
    }
    .partner_3 {
      width: 188px;
      height: 2px;
      background: #facc09;
      margin: 0 auto;
      margin-top: 3px;
    }
    .partner_4 {
      width: 38px;
      height: 2px;
      background: #00ffff;
      margin: 0 auto;
      margin-top: 3px;
    }
  }
  .partner .partner-img {
    margin-left: 437px;
  }

  .partner content {
    width: 80px;
    height: 200px;
    background: red;
    // margin: 0 auto;
  }

  .partner header img {
    display: block;
    margin: 0 auto;
  }

  .aboutUs {
    width: 100%;
    height: 640px;
    background: url('../../static/images/关于我们.png');
    padding-top: 95px;
  }

    .aboutUs header {
    width: 100%;
    height: auto;
    margin: 0 0 58px 0;
    text-align: center;
    .partner_1 {
      width: 145px;
      height: 34px;
      font-size: 36px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(41, 41, 41, 1);
    }
    .partner_2 {
      width: 140px;
      height: 13px;
      font-size: 16px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(41, 41, 41, 1);
    }
    .partner_3 {
      width: 188px;
      height: 2px;
      background: #facc09;
      margin: 0 auto;
      margin-top: 3px;
    }
    .partner_4 {
      width: 38px;
      height: 2px;
      background: #00ffff;
      margin: 0 auto;
      margin-top: 3px;
    }
  }

  .aboutUs header img {
    display: block;
    margin: 0 auto;
  }

  .aboutUs content {
    display: block;
    margin: 0 auto;
    width: 1106px;
    height: 430px;
    // background: red;
  }

  .aboutUs content p {
    text-indent: 2em;
    font-size: 20px;
    font-family: PingFang-SC-Medium;
    font-weight: 500;
    color: rgba(23, 42, 136, 1);
    line-height: 48px;
  }

  .box-img-black {
    height: 200px;
    background: url("../../static/image/choose-bottom-bg.png") 50% 50%;
  }
  .index-container {
    margin-top: 50px;
    background: #fff;
  }
}
</style>


