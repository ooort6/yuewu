<template>
  <div class="display">
    <div>
      <div class="display_1">
        <ul>
          <div class="display_3" v-for="(item,index) in items " :key="item.id">
            <span :class="{active:index==ins}" @click="activeShow(index)">
              {{item.id}}
              <span :class="index==ins?'arrowdown':'arrowright'"></span>
              <!-- <span class="arrowright"></span> -->
            </span>
            <div class="display_2" v-show="ins==index">
              <div v-show="index==0">
                <span v-for="(item,index1) in items1" :key="item.id" @click="spanShow1(index1)">
                  <a
                    :href="item.url"
                    class="display_4"
                    :class="{display_5:index1==ins1}"
                  >{{item.id}}</a>
                </span>
              </div>
              <div v-show="index==1">
                <span v-for="(item,index2) in items2" :key="item.id" @click="spanShow2(index2)">
                  <a
                    :href="item.url"
                    class="display_4"
                    :class="{display_5:index2==ins2}"
                  >{{item.id}}</a>
                </span>
              </div>
              <div v-show="index==2">
                <span v-for="(item,index3) in items3" :key="item.id" @click="spanShow3(index3)">
                  <a
                    :href="item.url"
                    class="display_4"
                    :class="{display_5:index3==ins3}"
                  >{{item.id}}</a>
                </span>
              </div>
            </div>
          </div>
        </ul>
        <div class="content_r" v-show="ins==0">
          <div class="content_1">
            <div style="width:993px;height:334px;margin-bottom:65px;">
              <div class="content_2">
                <span class="content_3"></span>
                <span class="content_4">可视化的商业数据展示</span>
                <br>
                <br>
                <br>
                <span class="content_6">
                  将您的数据可视化，并通过互动的界面展示给用户，
                  通过多点触摸界面，用户可以轻松了解海量数据信息，
                  并且可以十分直观的对数据进行分析操作。
                </span>
                <div class="content_2">
                  <span class="content_3"></span>
                  <span class="content_4">产品以及服务的展示</span>
                  <br>
                  <br>
                  <br>
                  <span class="content_6" style="margin-bottom:0">无论在任何行业，只要您需要对您的产品进行展示，</span>
                  <p class="content_7">多点触摸产品永远都是您最好的选择：直观、互动。展会、商场、零售商店...都是多点触摸产品的用武之地。</p>
                </div>
              </div>

              <div class="content_5">
                <img src="../../../static/images/fn4.jpg" alt>
              </div>
            </div>

            <div class="content_9">
              <span class="content_3"></span>
              <span class="content_4">3D互动设计</span>
            </div>
            <p class="content_8">多点触摸技术可以帮助您更好、更方便的呈现、控制和分析您的3D模型。</p>
            <p
              class="content_8"
              style="margin-bottom:84px"
            >作为3D设计的未来趋势，多点触摸在CAD、汽车、航空、制造业、房地产以及医疗等行业中都有很大的适用空间。</p>

            <div class="content_9">
              <span class="content_3"></span>
              <span class="content_4">集成式数字展牌</span>
            </div>
            <div id="zs"></div>
            <p class="content_8">通过使用带有网络连接的大型多点触摸屏幕（现在已经和普通LCD显示器一般大小）</p>
            <p class="content_8">作为大型展牌，可以实现网络化、集成化的管理，从而极大降低整体运营成本。</p>
          </div>

          <div class="content_zs">
            <img src="../../../static/images/fn5.jpg" alt>
            <div class="content_zs_1">
              <span class="content_zs_2">多媒体展示交互终端</span>
              <span class="content_zs_3">拥有多项业界领先的多点触控实现技术，满足不同场合和展示要求</span>
              <span
                class="content_zs_4"
              >它通过液晶显示屏幕或投影仪与交互传感器的双向整合， 利用各种网络，提供动画、视频、游戏等全方位的娱乐享受。是各品牌极佳的发布平台，受众只需轻触一块拥有触摸功能的显示屏，就可获取想关注的产品画面与信息。</span>
              <span class="content_zs_5">
                按照不同的触控实现技术，分为以下的不同系列
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">红外框多点触控系列</span>
                </div>
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">DI（散射光照明）多点触摸系列</span>
                </div>
                <div id="hy"></div>
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">全息纳米触控系列</span>
                </div>
              </span>
            </div>
          </div>

          <div class="content_hy">
            <span class="content_hy1">红外多点触控</span>
            <span class="content_hy2">使用红外多点触摸框，是目前最可靠、最便捷的多点触摸方案，可轻松安装在各种投影、液晶或等离子电视机上</span>
            <div class="content_hy3">
              <img src="../../../static/images/fn6.jpg" alt>
            </div>
            <div class="content_hy4">
              <span class="content_hy5"></span>
              <span class="content_hy6">特点:</span>
            </div>
            <div id="xn"></div>
            <span class="content_hy7">真多点触摸 安装轻松简易 无鬼点 低成本解决方案 抗干扰性强 可做二次开发</span>
          </div>

          <div class="content_xn">
            <span class="content_xn1">虚拟试衣镜</span>
            <span class="content_xn2">
              基于最新虚拟现实技术和测控技术的高档时尚电子产品，虚拟试衣系统通过全高清摄像头实时捕捉现场影像，并结合体感探测装置将服装的2D图片或3D模型叠加到顾客的影像上，实现虚拟服装与真实顾客身形的完美融合。
              <br>触角体感试衣镜可以让顾客用最短时间快速浏览不同服装款式的试穿效果，实现高效率的服装挑选，提升品牌的店内购物体验。同时，体感试衣镜还可以作为商场内的互动广告平台，实现有目标性的广告投放，并通过互动方式收集顾客反馈，为商场内不同品牌提供一个全新的产品展示与体验空间。
              <br>模拟真实试衣镜场景，红外测控技术在当参观者站在屏幕前的时候，通过专业的图形服务器计算后，虚拟试衣镜会自动将动态的具有特色的民俗服装试穿在参观者的身上，还可以更换不同的衣服款式，给你身临其境的感觉。
            </span>
            <div class="content_xn3">
              <span class="content_xn5"></span>
              <span class="content_xn4">特点:</span>
              <div class="content_xn6">
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">基于体感动作捕捉的自然交互方式</span>
                </div>
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">虚拟服装大小随试衣者身形自动适配</span>
                </div>
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">服装支持通过系列或款式分类，方便快速选择</span>
                </div>
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">支持同款服装不同颜色的快速切换</span>
                </div>
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">支持不同服饰的搭配效果</span>
                </div>
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">没顾客试衣时，支持自定义海报自动播放功能</span>
                </div>
                <div class="content_zs_6">
                  <i class="content_zs_7"></i>
                  <span class="content_zs_8">提供制作模板，允许用户自主快速制作并更新2D服装素材</span>
                </div>
              </div>
            </div>

            <img class="content_xn8" src="../../../static/images/fn7.jpg" alt>

            <div class="content_xn7">
              <span class="content_xn5"></span>
              <div id="mj"></div>
              <span class="content_xn4">应用范围:</span>
            </div>

            <p class="content_xn9">可广泛应用于商场、展览馆、婚博会、演艺现场、服装show、服装巡展等场所。</p>
          </div>

          <div class="content_mj">
            <span class="content_xn1">互动魔镜</span>
            <span
              class="content_xn2"
            >互动魔镜系统采用特殊材质镜面玻璃作为投影介质，投影机背投架设。参观者不仅可以照镜子，同时能看到高画质投影的3D立体影像，还可以用手触摸镜子表面，选择感兴趣的内容，镜面内的投影内容会被触发并与参观者形成互动。如一定时间内无人触摸时，系统可自动播放设置好的信息内容，当有人触摸时，则自动切换为互动式信息展示状态，给人一种梦幻的感觉。</span>

            <img class="content_mj1" src="../../../static/images/fn8.jpg" alt>
            <div id="cc"></div>
          </div>

          <div class="content_mj">
            <span class="content_xn1">互动橱窗</span>
            <span
              class="content_xn2"
              style="height:90px"
            >互动橱窗系统是利用投影设备将图像投射到玻璃橱窗的普通玻璃上，顾客通过手指在橱窗外玻璃上触摸点击、拖动等控制图像，阅读文字、欣赏图片及观看视频，体验神秘和魔术般的感觉。</span>
            <img class="content_mj1" src="../../../static/images/fn1.jpg" alt>
            <div id="bt"></div>
          </div>

          <div class="content_mj" style="height:550px">
            <span class="content_xn1">互动吧台</span>
            <span
              class="content_xn2"
              style="height:90px"
            >互动吧台系统是把互动投影与多点触控技术相结合，让普通桌面立刻变成一个多媒体互动娱乐游戏平台，图文并茂，形式新颖。参观者只需轻轻挥动手臂或触摸屏幕，就能观赏图像或参与游戏。</span>
            <img class="content_mj1" src="../../../static/images/fn2.jpg" alt>
            <div id="lt"></div>
          </div>

          <div class="content_lt">
            <span class="content_xn1">透明显示器，裸眼三维立体特效展示</span>
            <span
              class="content_lt1"
            >该产品利用橱窗内的灯光照明，为液晶板提供光源支持。支持触控操作，实现实时互动。鸿冠推出的彩色透明液晶显示屏采用宽视角技术，具有全高清、宽视角和高对比度等特色，可将具有高清分辨率的立体动感画面成像于透明空间。此外，还可通过遥控器开关控制，实现透明显示与正常显示的随意切换，具有很强的实用性和互动性，显示效果已达到同行业领先水平。</span>
            <img src="../../../static/images/fn3.jpg" alt>
          </div>
        </div>

        <div class="hdty" v-show="ins==1">
          <img class="hdty1" src="../../../static/images/1ty.jpg" alt>
          <div id="wm"></div>
          <div id="sm"></div>
          <div id="zqhd"></div>
          <div id="hdfs"></div>
          <div id="hdqmt"></div>
          <img class="hdty1" src="../../../static/images/2ty.jpg" alt>
          <img class="hdty1" src="../../../static/images/3ty.jpg" alt>
          <img class="hdty1" src="../../../static/images/4ty.jpg" alt>
          <img class="hdty1" src="../../../static/images/5ty.jpg" alt>
          <img class="hdty1" src="../../../static/images/6ty.jpg" alt>
        </div>

   <div class="dzsp" v-show="ins==2">
          <div id="sp"></div>
          <div id="bjh"></div>
      
          <img class="hdty1" src="../../../static/images/1sp.jpg" alt>
          <img class="hdty1" src="../../../static/images/2sp.jpg" alt>
          <img class="hdty1" src="../../../static/images/3sp.jpg" alt>
      
        </div>

      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "display",
  data() {
    return {
      index: 0,
      index1: 0,
      index2: 0,
      index3: 0,
      theme2: "light",
      ins: 3,
      ins1: 0,
      ins2: 0,
      ins3: 0,
      items: [
        { id: "多点触控软硬件解决方案" },
        { id: "互动投影" },
        { id: "电子沙盘系统" },
        { id: "投影拼接融合 " },
        { id: "虚拟成像" },
        { id: "识别系统" },
        { id: "增强现实 " }
      ],
      items1: [
        { id: "多媒体展示交互终端", url: "#zs" },
        { id: "红外多点触控", url: "#hy" },
        { id: "虚拟试衣镜 ", url: "#xn" },
        { id: "互动魔镜 ", url: "#mj" },
        { id: "互动橱窗 ", url: "#cc" },
        { id: "互动吧台 ", url: "#bt" },
        { id: "裸眼三维立体特效展示 ", url: "#lt" }
      ],
      items2: [
        { id: "雾幕系统", url: "#wm" },
        { id: "纱幕", url: "#sm" },
        { id: "桌面 墙面互动", url: "#zqhd" },
        { id: "互动翻书", url: "#hdfs" },
        { id: "互动签名台", url: "#hdqmt" }
      ],
      items3: [
        { id: "背光式数字沙盘", url: "#sp" },
        { id: "半景画  ", url: "#bjh" }
      ],
      header_content: [
        {
          id: "资源统一管理 ",
          content:
            "对馆内环境资源、设备资源、网络资源、应用资源、内容资源、电力资源六大类资源进行统一管理；提供资源统一视图快速检索资源；",
          img: require("../../../static/images/kz组 5.png")
        },
        {
          id: "智能调度控制 ",
          content:
            "通过移动终端或PC完成多终端内容快速智能调度，实现针对展示设备的展示内容可视化推送；对馆内设备、网络、电力等各类资源统一控制；",
          img: require("../../../static/images/kz组 4.png")
        },
        {
          id: "状态实时监控 ",
          content:
            "基于对展馆内的资源统一管理实时获取资源运行数据及状态，并提供可视化监控视图；异常监控数据实时告警并结合设备控制及时处理故障；",
          img: require("../../../static/images/kz组 2.png")
        },
        {
          id: "快速灵活布展 ",
          content:
            "提供展示主题策略配置，多类展示主线预先配置，灵活切换；基于云计算技术构建平台，满足外出快速灵活布展需求；",
          img: require("../../../static/images/kz组 3.png")
        }
      ]
    };
  },
  methods: {
    activeShow(index) {
      this.ins = index;
      this.index = index;
    },
    spanShow1(index1) {
      this.ins1 = index1;
      this.index1 = index1;
    },
    spanShow2(index2) {
      this.ins2 = index2;
      this.index2 = index2;
    },
    spanShow3(index3) {
      this.ins3 = index3;
      this.index3 = index3;
    },
       spanShow4(index4) {
      this.ins4 = index4;
      this.index4 = index4;
    },
       spanShow5(index5) {
      this.ins5 = index5;
      this.index5 = index5;
    },
       spanShow6(index6) {
      this.ins6 = index6;
      this.index6 = index6;
    },
       spanShow7(index7) {
      this.ins7 = index7;
      this.index7 = index7;
    },
    liClick(index) {
      this.isLiclick = index;

      // console.log(isLiclick)
    }
  },
  mounted() {}
};
</script>
<style lang="scss" scoped>
.display {
  background: #f9f9f9;
  // height: 5400px;
  padding-top: 5%;
  // width: 200px;
  // background: red;

  // ul{
  //     height: 1500px;
  //      float: left;
  //     margin-right: 2%;
  //     border-radius: 2%;
  //     margin-left: 300px;
  //     width: 346px;
  //     // height: 90%;
  //     background: #fff;

  // }

  .display_1 {
    height: 920px;
    // position: fixed;
    .display_2 {
      display: block;
      // float: left;
      // background: red;
      margin-bottom: 5%;
      padding-top: 10px;
      .display_4 {
        display: block;
        // background: red;
        margin-bottom: 5px;
        margin-top: 5px;
        // padding-top: 26px;
        padding-left: 26px;
        font-size: 18px;
        font-family: PingFang-SC-Medium;
        font-weight: 500;
        color: #737373;
      }
      .display_5 {
        display: block;
        // background: red;
        margin-bottom: 5px;
        margin-top: 5px;
        padding-left: 26px;
        font-size: 18px;
        font-family: PingFang-SC-Medium;
        font-weight: 500;
        color: #ffc738;
      }
    }
    ul {
      // position: fixed;
      float: left;
      margin-right: 2%;
      border-radius: 2%;
      margin-left: 300px;
      width: 346px;
      height: 90%;
      background: #fffcfc;
      padding-top: 2%;

      // background: red;
      .display_3 {
        padding-top: 3%;
        // height: 47px;
        display: block;

        span {
          display: block;
          // float: left;
          padding-left: 5%;
          font-size: 24px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
          // margin-bottom: 3%;
          cursor: pointer;
        }
        .arrowdown {
          width: 12px;
          height: 12px;
          display: inline;
          float: right;
          margin-right: 3%;
          margin-top: 4%;
          background: url("../../../static/images/jsdown.png") no-repeat;
        }
        .arrowright {
          width: 12px;
          height: 12px;
          display: inline;
          float: right;
          margin-right: 3%;
          margin-top: 4%;
          background: url("../../../static/images/jsright.png") no-repeat;
        }
        .active {
          background: #f1f1f1;
        }
      }
    }
    .content_r {
      width: 1015px;
      float: left;
      height: 5333px;
      margin-right: 25px;
      // background: red;
      .content_1 {
        width: 1015px;
        height: 825px;
        background: rgba(255, 252, 252, 1);
        box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
        border-radius: 10px;
        padding-top: 86px;
        padding-left: 28px;
        margin-bottom: 80px;
        .content_2 {
          width: 439px;
          height: 50px;
          float: left;
          .content_3 {
            display: block;
            float: left;
            width: 7px;
            height: 28px;
            background: rgba(255, 199, 56, 1);
            margin-right: 7px;
          }
          .content_4 {
            width: 310px;
            height: 29px;
            margin-top: -10px;
            display: block;
            float: left;
            font-size: 30px;
            font-family: PingFang-SC-Medium;
            // font-weight:500;
            color: rgba(38, 32, 34, 1);
            margin-bottom: 35px;
          }
          .content_6 {
            display: block;
            margin-left: 16px;
            font-size: 18px;
            font-family: PingFang-SC-Regular;
            font-weight: 400;
            color: rgba(38, 32, 34, 1);
            margin-bottom: 69px;
          }
          .content_7 {
            width: 892px;
            display: block;
            margin-left: 16px;
            font-size: 18px;
            font-family: PingFang-SC-Regular;
            font-weight: 400;
            color: rgba(38, 32, 34, 1);
            // margin-bottom: 185px;
          }
        }
        .content_5 {
          margin-left: 65px;
          display: block;
          float: left;
          width: 421px;
          height: 282px;
          // background: red;
        }
        .content_9 {
          width: 1015px;
          height: 50px;
          float: left;
          .content_3 {
            display: block;
            float: left;
            width: 7px;
            height: 28px;
            background: rgba(255, 199, 56, 1);
            margin-right: 7px;
          }
          .content_4 {
            width: 310px;
            height: 29px;
            margin-top: -10px;
            display: block;
            float: left;
            font-size: 30px;
            font-family: PingFang-SC-Medium;
            // font-weight:500;
            color: rgba(38, 32, 34, 1);
            margin-bottom: 35px;
          }
        }
        .content_8 {
          padding-left: 16px;
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(38, 32, 34, 1);
          // background: red;
        }
      }

      .content_zs {
        width: 1015px;
        height: 497px;
        background: rgba(255, 252, 252, 1);
        box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
        border-radius: 10px;
        padding-top: 40px;
        padding-left: 28px;
        margin-bottom: 43px;
        img {
          display: block;
          float: left;
          margin-right: 50px;
        }
        .content_zs_1 {
          float: left;

          width: 571px;
          height: 402px;
          // background: red;
          .content_zs_2 {
            display: block;
            text-align: center;
            font-size: 30px;
            font-family: PingFang-SC-Medium;
            font-weight: 500;
            color: rgba(38, 32, 34, 1);
            margin-bottom: 16px;
          }
          .content_zs_3 {
            display: block;
            width: 562px;
            background: rgba(255, 199, 56, 0.1);
            font-size: 18px;
            font-family: PingFang-SC-Regular;
            font-weight: 400;
            color: rgba(38, 32, 34, 1);
            margin-bottom: 53px;
          }
          .content_zs_4 {
            display: block;
            width: 571px;
            height: 111px;
            font-size: 18px;
            font-family: PingFang-SC-Regular;
            font-weight: 400;
            color: rgba(38, 32, 34, 1);
            margin-bottom: 42px;
          }
          .content_zs_5 {
            display: block;
            height: 112px;
            // background: red;
            font-size: 18px;
            font-family: PingFang-SC-Regular;
            font-weight: 400;
            color: rgba(38, 32, 34, 1);
            .content_zs_6 {
              height: 30px;

              // background: #ffc738;
              .content_zs_7 {
                display: block;
                border-radius: 50%;
                width: 10px;
                height: 10px;
                background: #ffc738;
                float: left;
                margin-top: 9px;
                margin-right: 16px;
              }
              .content_zs_8 {
                font-size: 18px;
                font-family: PingFang-SC-Regular;
                font-weight: 400;
                color: rgba(38, 32, 34, 1);
              }
            }
          }
        }
      }

      .content_hy {
        width: 1015px;
        height: 484px;
        background: rgba(255, 252, 252, 1);
        box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
        border-radius: 10px;
        padding-top: 40px;
        margin-bottom: 46px;
        // padding-left: 28px;
        .content_hy1 {
          display: block;
          text-align: center;
          margin-bottom: 17px;
          font-size: 30px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
        }
        .content_hy2 {
          display: block;
          text-align: center;
          margin-bottom: 53px;
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(38, 32, 34, 1);
        }
        .content_hy3 {
          text-align: center;
        }
        .content_hy4 {
          margin-top: 10px;
          width: 1015px;
          height: 30px;
          margin-bottom: 25px;

          .content_hy5 {
            display: block;
            float: left;
            width: 7px;
            height: 25px;
            background: #ffc738;
            margin-left: 60px;
            margin-right: 7px;
          }
          .content_hy6 {
            display: block;
            margin-top: -6px;

            float: left;
            font-size: 24px;
            font-family: PingFang-SC-Medium;
            font-weight: 500;
            color: rgba(38, 32, 34, 1);
          }
        }

        .content_hy7 {
          display: block;
          font-size: 18px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
          margin-left: 103px;
        }
      }

      .content_xn {
        width: 1015px;
        height: 921px;
        background: rgba(255, 252, 252, 1);
        box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
        border-radius: 10px;
        padding-top: 60px;
        .content_xn1 {
          display: block;
          text-align: center;
          margin-bottom: 40px;
          font-size: 30px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
        }
        .content_xn2 {
          width: 887px;
          height: 240px;
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(38, 32, 34, 1);
          display: block;
          margin: 0 auto;
        }
        .content_xn3 {
          width: 556px;
          height: 289px;
          float: left;
          // background: greenyellow;
          margin-left: 6%;
          .content_xn4 {
            display: block;
            margin-top: -6px;

            float: left;
            font-size: 24px;
            font-family: PingFang-SC-Medium;
            font-weight: 500;
            color: rgba(38, 32, 34, 1);
          }
          .content_xn5 {
            display: block;
            float: left;
            width: 7px;
            height: 25px;
            background: #ffc738;
            // margin-left: 35px;
            margin-right: 7px;
          }
          .content_xn6 {
            width: 489px;
            height: 208px;
            background: #fff;
            float: right;
            margin-top: 38px;
            .content_zs_6 {
              height: 30px;

              // background: #ffc738;
              .content_zs_7 {
                display: block;
                border-radius: 50%;
                width: 10px;
                height: 10px;
                background: #ffc738;
                float: left;
                margin-top: 9px;
                margin-right: 16px;
              }
              .content_zs_8 {
                font-size: 18px;
                font-family: PingFang-SC-Regular;
                font-weight: 400;
                color: rgba(38, 32, 34, 1);
              }
            }
          }
        }
        .content_xn8 {
          display: block;
          float: left;
          margin-left: 4%;
        }
        .content_xn7 {
          width: 584px;
          height: 52px;
          float: left;
          margin-left: 6%;
          margin-bottom: 20px;

          .content_xn4 {
            display: block;
            margin-top: -6px;

            float: left;
            font-size: 24px;
            font-family: PingFang-SC-Medium;
            font-weight: 500;
            color: rgba(38, 32, 34, 1);
          }
          .content_xn5 {
            display: block;
            float: left;
            width: 7px;
            height: 25px;
            background: #ffc738;
            // margin-left: 35px;
            margin-right: 7px;
          }
        }
        .content_xn9 {
          display: block;
          float: left;
          font-size: 18px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
          margin-left: 120px;
        }
      }

      .content_mj {
        width: 1015px;
        height: 577px;
        background: rgba(255, 252, 252, 1);
        box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
        border-radius: 10px;
        padding-top: 40px;
        margin-top: 49px;
        .content_xn1 {
          display: block;
          text-align: center;
          margin-bottom: 30px;
          font-size: 30px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
        }
        .content_xn2 {
          width: 887px;
          height: 150px;
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(38, 32, 34, 1);
          display: block;
          margin: 0 auto;
          // margin-bottom: 50px;
        }
        .content_mj1 {
          display: block;
          margin: 0 auto;
        }
      }

      .content_lt {
        width: 1015px;
        height: 449px;
        background: rgba(255, 252, 252, 1);
        box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
        border-radius: 10px;
        padding-top: 40px;
        margin-top: 49px;
        .content_xn1 {
          display: block;
          text-align: center;
          margin-bottom: 30px;
          font-size: 30px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
        }
        .content_lt1 {
          width: 452px;
          height: 205px;
          // background: #ffc738;
          float: left;
          margin-left: 38px;
          margin-right: 33px;
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(38, 32, 34, 1);
        }
      }
    }

    .hdty {
      width: 1015px;
      float: left;
      height: 4777px;
      margin-right: 25px;
      // background: red;
      // .content_1 {
      //   width: 1015px;
      //   height: 961px;
      //   background: rgba(255, 252, 252, 1);
      //   box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
      //   border-radius: 10px;
      //   padding-top: 40px;
      //   padding-left: 49px;
      //   margin-bottom: 80px;
      //   .content_2 {
      //     display: block;
      //     width: 868px;
      //     height: 112px;
      //     font-size: 18px;
      //     font-family: PingFang-SC-Regular;
      //     font-weight: 400;
      //     color: rgba(38, 32, 34, 1);
      //   }
      // }
      .hdty1 {
        background: rgba(255, 252, 252, 1);
        box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
        border-radius: 10px;
        margin-bottom: 40px;
        // border: none;
        // padding: 0;
      }
      #wm {
        position: absolute;
        top: 1000px;
      }
      #sm {
        position: absolute;
        top: 1880px;
      }
      #zqhd {
        position: absolute;
        top: 2680px;
      }
      #hdfs {
        position: absolute;
        top: 3430px;
      }
      #hdqmt {
        position: absolute;
        top: 4100px;
      }
    }

.dzsp {
      width: 1015px;
      float: left;
      height: 3400px;
      margin-right: 25px;
      // background: red;
      // .content_1 {
      //   width: 1015px;
      //   height: 961px;
      //   background: rgba(255, 252, 252, 1);
      //   box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
      //   border-radius: 10px;
      //   padding-top: 40px;
      //   padding-left: 49px;
      //   margin-bottom: 80px;
      //   .content_2 {
      //     display: block;
      //     width: 868px;
      //     height: 112px;
      //     font-size: 18px;
      //     font-family: PingFang-SC-Regular;
      //     font-weight: 400;
      //     color: rgba(38, 32, 34, 1);
      //   }
      // }
      .hdty1 {
        background: rgba(255, 252, 252, 1);
        box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
        border-radius: 10px;
        margin-bottom: 40px;
        // border: none;
        // padding: 0;
      }
      #sp {
        position: absolute;
        top: 1900px;
      }
      #bjh {
        position: absolute;
        top: 2700px;
      }
    
    }


  }
}
</style>

