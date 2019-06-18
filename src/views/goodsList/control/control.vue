<template>
  <div class="control">
    <div>
      <div class="content_l">
        <ul>
          <li v-for="(item,index) in items " :key="item.id">
            <span :class="{active:index==ins}"  @click="activeShow(index)">{{item.id}}</span>
          </li>
        </ul>
        <div class="content_r" v-show="ins==0">
          <img src="../../../static/images/kz表格1.png" alt>
          <div class="content_r_header">
            <div class="header_content" v-for="(item) in header_content" :key="item.id">
              <img :src="item.img" alt>
              <span class="header_1">{{item.id}}</span>
              <p class="header_2">{{item.content}}</p>
              <!-- {{item.img_add}} -->
            </div>
          </div>

          <div class="content_r_content">
            <div class="content_1"></div>
            <span class="content_2">集中控制系统：</span>
            <p class="content_3">
              集中控制系统是指对声、光、电等各种硬件设备进行集中控制的完整解决方案，
              <br>将一特定环境中需要控制的设备通过一定的网络连接到一起，开发集中控制软件，
              <br>来对各个设备进行统一的管理。它应用于各种展厅、多媒体教室、多功能会议厅、指挥控制中心、智能化家庭等，
              <br>用户可使用显示设备，通过集中控制系统软件控制投影机、展示台、液晶电视、计算机、笔记本、灯光等设备的开关，
              还可以对可调灯光进行灯光亮度的调节。
            </p>
            <div class="content_4">
              <span>系统特点</span>
            </div>
            <div class="content_5">
              <i class="content_5_2"></i>
              <p class="content_5_1">提供多种控制接口，开发者可以开发运行于各种显示终端的控制界面来作为交互界面。</p>
            </div>
            <div class="content_5">
              <i class="content_5_2"></i>
              <p class="content_5_1">使用Ipad进行控制，交互体验效果好。</p>
            </div>
            <div class="content_5">
              <i class="content_5_2"></i>
              <p class="content_5_1">能同时对多路设备进行控制。在控制投影机进行演播同时，能对灯光进行调光控制，达到更好的观影效果。</p>
            </div>
            <div class="content_5">
              <i class="content_5_2"></i>
              <p class="content_5_1">集成度高，设备控制方式齐全，系统扩展功能强，可靠性高等特点。低成本，高性能，高集成度，全数字化控制。</p>
            </div>
          </div>
        </div>

        <div id="DW" v-show="ins==1">
          <div class="dw">
            <img src="../../../static/images/zn表格.png" alt>
            <span class="content_1">高精度无线定位系统包括:</span>
            <p class="content_2">1.定位硬件层：定位微基站和定位微标签</p>
            <p class="content_2">2.网络连接层：连接基站且传送采集数据至定位解算中心</p>
            <p class="content_2">3.数据解算层：计算标签位置</p>
            <p class="content_2">4.应用层：客户定制应用呈现</p>
          </div>

          <div class="dw1">
            <span class="content_1">系统功能</span>
            <p class="content_2">展览馆内通常需要对来访人员进行统计和贵重物品跟踪，为馆方提供可靠的人员行走分析及物品定位，可以提高展馆的有效性和科技含量。</p>
            <p
              class="content_2"
            >展厅人员定位解决方案，采用超宽带（UWB）实时定位系统。通过在展馆内布设一定数量的基站Anchor），实时精确地定位人员佩戴的标签（Tag），准确实时地将人员的位置信息反馈到监控中心，方便管理人员监控、调度以及后期行为分析等，该系统精度最高可达到10cm。</p>
            <div class="content_3">
              <div class="content_4">
                <img class="content_6" src="../../../static/images/zn1.png" alt>
                <span class="content_5">实时位置定位</span>
                <p class="content_7">使用者能关注重点区域的人员实时分布情况</p>
                <p class="content_7">满足不同定位需求：存在性检测、1D、2D、3D</p>
              </div>
              <div class="content_4">
                <img class="content_6" src="../../../static/images/zn2.png" alt>
                <span class="content_5">电子栅栏功能</span>
                <p class="content_7">定位目标进入禁区，如危险区或涉密区等</p>
                <p class="content_7">严控范围，系统报警，提供管理参考</p>
              </div>
              <div class="content_4">
                <img class="content_6" src="../../../static/images/zn3.png" alt>
                <span class="content_5">突发情况报警</span>
                <p class="content_7">定位目标遇突发情况按下标签设备的定位按钮，</p>
                <p class="content_7">监控画面立即触发报警时间并纪录</p>
              </div>
              <div class="content_4">
                <img class="content_6" src="../../../static/images/zn4.png" alt>
                <span class="content_5">统计与查询</span>
                <p class="content_7">管理者可查看任意区域、任何目标信息状况，</p>
                <p class="content_7">支持历史数据查询、支持统计与报表打印</p>
              </div>
            </div>
          </div>

          <div class="dw2">
            <span class="content_1">应用场景</span>
            <div class="content_2">
              <span class="content_3">人员定位</span>
              <img class="content_4" src="../../../static/images/zn5.png" alt>
              <p class="content_5">工厂、监狱、监所人员定位 / 隧道、矿山人员定位系统 / 变电站巡检员定位系统</p>
              <br>
              <p class="content_5">安保人员在岗与定位监测 / 老人、儿童、宠物看护系统 / 定点驱动军事训练系统</p>
            </div>
            <div class="content_2">
              <span class="content_3">设备定位</span>
              <img class="content_4" src="../../../static/images/zn6.png" alt>
              <p class="content_5">重要物资定位系统 / 供应链管理与可视化离散制造</p>
              <br>
              <p class="content_5">库存与物流管理系统 / 工业AGV机器人定位系统</p>
            </div>
            <div class="content_2">
              <span class="content_3">综合定位</span>
              <img class="content_4" src="../../../static/images/zn7.png" alt>
              <p class="content_5">购物车导航与广告投放应用 / 医院人员、设备综合管理系统</p>
              <br>
              <p class="content_5">施工安全距离监测 / 物联网领域其他定位类用途</p>
            </div>
          </div>
        </div>

        <div id="FX" v-show="ins==2">
          <div class="fx">
            <div class="content_1">
              <span class="content_2"></span>
              <span class="content_4">基于云服务的组网方案</span>
              <p class="content_5">Network scheme based on cloud services</p>
              <span class="content_3"></span>
            </div>
            <img class="content_6" src="../../../static/images/kj表格.png" alt>
            <span class="content_7">(安防及视频智能分析开发平台)</span>
          </div>

          <div class="fx1">
            <div class="content_1">
              <span class="content_2"></span>
              <span class="content_4">能力汇总表</span>
              <p class="content_5">Capacity matrix</p>
              <span class="content_3"></span>
            </div>
            <div class="content_14">
              <div class="content_6">
                <img class="content_8" src="../../../static/images/kj1.png" alt>
                <span class="content_7">视频分析能力</span>
              </div>
              <div class="content_9">
                <div class="content_10">
                  <span class="content_11">客流分析能力</span>
                  <p class="content_12">经过区域的人流分析</p>
                  <p class="content_12">经过区域的人流分析</p>
                  <p class="content_12">经过区域的人流分析</p>
                </div>
                <div class="content_10">
                  <span class="content_11" style="margin-bottom:1%">行为能力</span>
                  <p class="content_12" style="margin-bottom:0%">进入警戒面分析</p>
                  <p class="content_12" style="margin-bottom:0%">进入区域分析</p>
                  <p class="content_12" style="margin-bottom:0%">在区域逗留分析</p>
                  <p class="content_12" style="margin-bottom:0%">停车分析</p>
                  <p class="content_12" style="margin-bottom:0%">离开区域分析</p>
                  <p class="content_12" style="margin-bottom:0%">区域入侵分析</p>
                </div>
                <div class="content_10">
                  <span class="content_11">车辆识别</span>
                  <p class="content_12">车辆信息识别</p>
                  <p class="content_12">实时车牌比对</p>
                  <p class="content_12">车牌查询</p>
                </div>
                <div class="content_10">
                  <span class="content_11">人脸识别</span>
                  <p class="content_12">黑名单告警</p>
                  <p class="content_12">人脸搜索</p>
                  <p class="content_12">人脸比对</p>
                </div>
              </div>
            </div>
            <div class="content_13">
              <img class="content_8" src="../../../static/images/kj2.png" alt>
              <span class="content_7">安防监控能力</span>

              <div class="content_15">
                <p class="content_12">消防监控能力</p>
                <p class="content_12">防盗入侵监控能力</p>
                <p class="content_12">电梯告警能力</p>
                <p class="content_12">门禁管理能力</p>
                <p class="content_12">电子围栏等等</p>
                <p class="content_12">视频实时监控</p>
                <p class="content_12">视频回看</p>
                <p class="content_12">摄像头管理</p>
              </div>
            </div>

            <div class="content_16">
              <img class="content_8" src="../../../static/images/kj3.png" alt>
              <span class="content_7">GIS地图能力</span>
              <div class="content_17">
                <p class="content_12">基于地图网络分析</p>
                <p class="content_12">电视墙展示</p>
              </div>
            </div>
            <div class="content_18">
              <div class="content_19">
                <img class="content_8" src="../../../static/images/kj4.png" alt>
                <span class="content_7">数据分析能力</span>
              </div>

              <div class="content_20">
                <p class="content_12">告警统计分析</p>
                <p class="content_12">日常数据监控</p>
              </div>
            </div>
          </div>

          <div class="fx3">
            <div class="content_1">
              <span class="content_2"></span>
              <span class="content_4">场景解决方案</span>
              <p class="content_5">Scenario solution</p>
              <span class="content_3"></span>
            </div>
            <div class="content_6">
              <img class="content_7" src="../../../static/images/kj组 28.png" alt>
              <span class="content_8">场景一: 人流车流监控管理</span>
              <div class="content_9">
                <img class="content_10" src="../../../static/images/kj图层 2.png" alt>
                <img class="content_11" src="../../../static/images/kj组 30.png" alt>
                <span class="content_12">人流异常预警</span>
                <span class="content_13">
                  通过视频监控和平台分析，
                  <br>发现人群异常聚集的区域并自动告警。
                </span>
              </div>

              <div class="content_9">
                <span class="content_14">小区群租管理</span>
                <span class="content_15">
                  通过对楼宇出入口视频监控分析或门禁系统管理，
                  <br>统计出入人员流量，及时预判群租并视频取证。
                </span>
                <img class="content_16" src="../../../static/images/kj图层 3.png" alt>

                <img class="content_17" src="../../../static/images/kj组 30 拷贝.png" alt>
              </div>

              <div class="content_9">
                <img class="content_10" src="../../../static/images/kj图层 4.png" alt>
                <img class="content_11" src="../../../static/images/kj组 30.png" alt>
                <span class="content_12">车流异常预警</span>
                <span class="content_13">
                  通过视频监控和平台分析，
                  <br>发现车流异常拥堵区域并自动告警。
                </span>
              </div>
            </div>
            <Divider style="background:#D2D2D2;min-width:60px;width:92%;"/>

            <div class="content_6">
              <img class="content_7" src="../../../static/images/kj组 28.png" alt>
              <span class="content_8">场景二: 区域边界监控管理</span>
              <div class="content_9">
                <img class="content_10" src="../../../static/images/kj图层 5.png" alt>
                <img class="content_11" src="../../../static/images/kj组 30.png" alt>
                <span class="content_12">占道经营管理</span>
                <span class="content_13">
                  通过对指定过道及区域的视频监控分析，
                  <br>发现违法占道经营并告警取证。
                </span>
              </div>

              <div class="content_9">
                <span class="content_14">违章搭建监控及管理</span>
                <span class="content_15">
                  针对重点位置或已发现违章搭建
                  <br>利用入侵检测技术进行监控取证
                </span>
                <img class="content_16" src="../../../static/images/kj图层 6.png" alt>

                <img class="content_17" src="../../../static/images/kj组 30 拷贝.png" alt>
              </div>

              <div class="content_9">
                <img class="content_10" src="../../../static/images/kj图层 7.png" alt>
                <img class="content_11" src="../../../static/images/kj组 30.png" alt>
                <span class="content_12">越界逗留侦测</span>
                <span class="content_13">
                  针对特定区域及边界，
                  <br>通过视频监控及分析发现越界或非法逗留人员或物体，
                  <br>及时告警并取证。
                </span>
              </div>
            </div>
            <Divider style="background:#D2D2D2;min-width:60px;width:92%;"/>
            <div class="content_6" style="height:590px">
              <img class="content_7" src="../../../static/images/kj组 28.png" alt>
              <span class="content_8">场景三: 小区出入口监控管理</span>
              <div class="content_9">
                <img class="content_10" src="../../../static/images/kj图层 8.png" alt>
                <img class="content_11" src="../../../static/images/kj组 30.png" alt>
                <span class="content_12">门禁监控管理</span>
                <span class="content_13">
                  通过人脸识别、RFID识别等技术
                  <br>实现对出入人员管理
                </span>
              </div>

              <div class="content_9">
                <span class="content_14">人员黑名单管理</span>
                <span class="content_15">
                  在出入口或重点区域，
                  <br>通过人脸识别技术
                  <br>实现对黑名单人员的发现、预警、跟踪及管理取证，
                  <br>
实现与周边监控探头的联动。
                </span>
                <img class="content_16" src="../../../static/images/kj图层 9.png" alt>

                <img class="content_17" src="../../../static/images/kj组 30 拷贝.png" alt>
              </div>
            </div>
            <Divider style="background:#D2D2D2;min-width:60px;width:92%;"/>
            <div class="content_6">
              <img class="content_7" src="../../../static/images/kj组 28.png" alt>
              <span class="content_8">场景四: 安防减灾管理</span>
              <div class="content_9">
                <img class="content_10" src="../../../static/images/kj图层 10.png" alt>
                <img class="content_11" src="../../../static/images/kj组 30.png" alt>
                <span class="content_12">消防实时监控</span>
                <span class="content_13">
                  利用烟雾感应、温度感应、视频监控等设备整合，
                  <br>自动发现并定位火警现场，
                  <br>并联动周边探头实现实时动态监测。
                </span>
              </div>

              <div class="content_9">
                <span class="content_14">电子围栏</span>
                <span class="content_15">
                  针对小区或重点场所围墙大范围边界
                  <br>
利用红外、视频、线圈等检测技术实现异常入侵告警
                </span>
                <img class="content_16" src="../../../static/images/kj图层 11.png" alt>

                <img class="content_17" src="../../../static/images/kj组 30 拷贝.png" alt>
              </div>

              <div class="content_9">
                <img class="content_10" src="../../../static/images/kj图层 12.png" alt>
                <img class="content_11" src="../../../static/images/kj组 30.png" alt>
                <span class="content_12">视频对讲</span>
                <span class="content_13">
                  基于单兵移动设备提供视频对讲，移动取证等功能
                  <br>用于补充视频监控死角。
                </span>
              </div>
            </div>
          </div>
        </div>

<div id="XY" v-show="ins==3">
 <img class="content_1" src="../../../static/images/xn.png" alt="">
 <span class="content_2">中国电信信息生活体验馆：<a style="color:#FACC09" href="https://www.infospace.sh.cn">https://www.infospace.sh.cn</a></span>
</div>

<div id="DL" v-show="ins==4">
      <div class="content_1">
        <span class="content_2">
          通过互动APP，结合高精度定位技术及中控系统，让参观嘉宾可以方便地自行参观，随时了解每个展项的信息（文本、声音及视频等），通过语音互动来实现互动参观（控制灯光、展示内容等），增强参观体验度。

        </span>
<img src="../../../static/images/zz.png" alt="">
      </div>

</div>

      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "control",
  data() {
    return {
      ins: 0,
      items: [
        { id: "智慧展厅控制系统" },
        { id: "高精度定位系统" },
        { id: "智能视频分析系统" },
        { id: "虚拟巡游系统" },
        { id: "自助导览系统" }
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
    }
  },
  mounted() {}
};
</script>
<style lang="scss" scoped>
.control {
  background: #f9f9f9;
  height: 2250px;
  padding-top: 5%;
  // width: 200px;
  // background: red;

  .content_l ul {
    float: left;
    margin-right: 2%;
    border-radius: 2%;
    margin-left: 300px;
    width: 346px;
    height: 2180px;
    background: #fff;
    // background: red;
  }
  .content_l ul li {
    padding-top: 10%;
    height: 47px;
    display: block;

    span {
      display: block;
      padding-left: 20%;
      font-size: 24px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(38, 32, 34, 1);
      margin-bottom: 3%;
      cursor: pointer;
    }
    .active {
      background: #f1f1f1;
    }
  }
  .content_r {
    // background: red;
    height: 2250px;
    width: 929px;
    float: left;

    .content_r_header {
      padding-left: 8.5%;
      padding-top: 7%;
      width: 929px;
      height: 747px;
      background: rgba(255, 252, 252, 1);
      box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
      border-radius: 10px 10px 0px 0px;
      margin-top: 4%;
      .header_content {
        height: 150px;
        img {
          float: left;
          margin-right: 2%;
        }
        .header_1 {
          font-size: 24px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
          float: left;
        }
        .header_2 {
          display: block;
          position: relative;
          top: 40%;
          left: -23%;
          font-size: 16px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
        }
      }
    }
    .content_r_content {
      // background: red;
      height: 30px;
      margin-top: 8%;
      .content_1 {
        width: 6px;
        height: 27px;
        background: #ffc738;
        float: left;
        margin-top: 1%;
        margin-left: 3%;
        margin-right: 5px;
      }
      .content_2 {
        font-size: 30px;
        font-family: PingFang-SC-Medium;
        font-weight: 500;
        color: rgba(38, 32, 34, 1);
      }
      .content_3 {
        width: 954px;
        margin-left: 3%;
        display: block;
        margin-top: 3%;
        font-size: 18px;
        font-family: PingFang-SC-Medium;
        font-weight: 500;
        color: rgba(38, 32, 34, 1);
      }
      .content_4 {
        width: 117px;
        height: 32px;
        background: rgba(255, 199, 56, 0.1);
        margin-left: 3%;
        margin-top: 4.3%;
        text-align: center;
        margin-bottom: 3%;
        span {
          font-size: 24px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
        }
      }
      .content_5 {
        width: 954px;
        margin-bottom: 2%;
        .content_5_1 {
          font-size: 18px;
          font-family: PingFang-SC-Medium;
          // font-weight:500;
          color: #262022;
        }
        .content_5_2 {
          display: block;
          width: 12px;
          height: 12px;
          background: #ffc738;
          border-radius: 50%;
          float: left;
          margin-top: 1%;
          margin-right: 1%;
          margin-left: 3%;
        }
      }
    }
  }
  .dw {
    width: 929px;
    float: left;
    padding-left: 3.5%;
    padding-top: 2%;
    height: 797px;
    background: rgba(255, 252, 252, 1);
    box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
    border-radius: 10px 10px 0px 0px;
    .content_1 {
      margin-top: 7.4%;
      display: block;
      width: 282px;
      height: 32px;
      // background: red;
      // padding-t
      font-size: 24px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(38, 32, 34, 1);
      border-bottom: 5px solid #facc09;
      margin-bottom: 4%;
    }
    .content_2 {
      font-size: 20px;
      font-family: PingFang-SC-Regular;
      font-weight: 400;
      color: rgba(38, 32, 34, 1);
      margin-bottom: 1%;
    }
  }
  .dw1 {
    width: 929px;
    margin-top: 2.6%;
    float: left;
    // padding-left: 3.5%;
    padding-top: 2%;
    height: 797px;
    background: rgba(255, 252, 252, 1);
    box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
    border-radius: 10px 10px 0px 0px;
    .content_1 {
      font-size: 36px;
      font-family: PingFang-SC-Bold;
      font-weight: bold;
      color: rgba(38, 32, 34, 1);
      text-align: center;
      display: block;
      margin-bottom: 3%;
    }
    .content_2 {
      display: block;
      margin-left: 9%;
      width: 779px;
      font-size: 18px;
      font-family: PingFang-SC-Regular;
      font-weight: 400;
      color: rgba(38, 32, 34, 1);
    }
    .content_3 {
      margin-top: 10%;
      width: 820px;
      // background: red;
      height: 388px;
      margin-left: 9%;
      .content_4 {
        padding-top: 3%;
        padding-left: 1.5%;
        width: 410px;
        height: 194px;
        float: left;
        .content_5 {
          display: block;
          float: left;
          font-size: 24px;
          font-family: PingFang-SC-Medium;
          font-weight: 500;
          color: rgba(38, 32, 34, 1);
        }
        .content_6 {
          display: block;
          float: left;
          margin-right: 2%;
        }
        .content_7 {
          margin-top: 6%;
          display: block;
          float: left;
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(38, 32, 34, 1);
          width: 379px;
          margin-bottom: -10px;
        }
      }
    }
  }
  .dw2 {
    width: 929px;
    margin-top: 2.6%;
    float: left;
    // padding-left: 3.5%;
    padding-top: 2%;
    height: 561px;
    background: rgba(255, 252, 252, 1);
    box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
    border-radius: 10px 10px 0px 0px;
    .content_1 {
      font-size: 36px;
      font-family: PingFang-SC-Bold;
      font-weight: bold;
      color: rgba(38, 32, 34, 1);
      text-align: center;
      display: block;
      margin-bottom: 3%;
    }
    .content_2 {
      margin-bottom: 8%;
      .content_3 {
        font-size: 24px;
        font-family: PingFang-SC-Medium;
        font-weight: 500;
        color: rgba(38, 32, 34, 1);
        text-align: center;
        display: block;
        margin-bottom: 2%;
      }
      .content_4 {
        float: left;
        margin-left: 9.5%;
        margin-right: 2.5%;
      }
      .content_5 {
        font-size: 18px;
        font-family: PingFang-SC-Regular;
        font-weight: 400;
        color: rgba(38, 32, 34, 1);
        display: block;
        float: left;
        margin-bottom: 1%;
      }
    }
  }
  .fx {
    width: 929px;
    float: left;
    padding-left: 3.5%;
    padding-top: 2%;
    height: 797px;
    background: rgba(255, 252, 252, 1);
    box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
    border-radius: 10px 10px 0px 0px;
    margin-bottom: 35px;
    .content_1 {
      width: 315px;
      // background: red;
      height: 40px;
      margin: 0 auto;
      margin-bottom: 6%;
    }
    .content_2 {
      display: block;
      width: 17.5px;
      height: 35px;
      float: left;
      // padding-top:2%;
      border: 3px solid #646061;
      border-right: none;
    }
    .content_3 {
      display: block;
      width: 17.5px;
      height: 35px;
      float: left;
      margin-top: -7.5%;
      margin-left: 6.5%;
      // padding-top:2%;
      border: 3px solid #646061;
      border-left: none;
    }
    .content_4 {
      display: block;
      float: left;
      margin-left: 6%;
      margin-top: -4%;
      font-size: 24px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(38, 32, 34, 1);
    }
    .content_5 {
      display: block;
      float: left;
      margin-left: 7%;
      font-size: 12px;
      font-family: PingFang-SC-Regular;
      font-weight: 400;
      color: rgba(38, 32, 34, 1);
    }
    .content_6 {
      display: block;
      margin: 0 auto;
      margin-bottom: 5%;
    }
    .content_7 {
      display: block;
      text-align: center;
      font-size: 18px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(78, 78, 78, 1);
    }
  }
  .fx1 {
    width: 929px;
    float: left;
    padding-left: 3.5%;
    padding-top: 2%;
    height: 918px;
    background: rgba(255, 252, 252, 1);
    box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
    border-radius: 10px 10px 0px 0px;
    margin-bottom: 35px;
    .content_1 {
      width: 175px;
      // background: red;
      height: 40px;
      margin: 0 auto;
      margin-bottom: 6%;
    }
    .content_2 {
      display: block;
      width: 17.5px;
      height: 35px;
      float: left;
      // padding-top:2%;
      border: 3px solid #646061;
      border-right: none;
    }
    .content_3 {
      display: block;
      width: 17.5px;
      height: 35px;
      float: right;
      margin-top: -16.5%;
      // margin-left: 8.5%;
      // padding-top:2%;
      border: 3px solid #646061;
      border-left: none;
    }
    .content_4 {
      display: block;
      float: left;
      margin-left: 6%;
      margin-top: -4%;
      font-size: 24px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(38, 32, 34, 1);
    }
    .content_5 {
      display: block;
      float: left;
      margin-left: 12%;
      font-size: 12px;
      font-family: PingFang-SC-Regular;
      font-weight: 400;
      color: rgba(38, 32, 34, 1);
    }
    .content_6 {
      width: 439px;
      height: 97px;
      float: left;
      // background: red;
    }
    .content_7 {
      display: block;
      float: left;
      margin-top: 5%;
      font-size: 24px;
      font-family: PingFang-SC-Bold;
      font-weight: bold;
      color: rgba(0, 0, 0, 1);
    }
    .content_8 {
      float: left;
      margin-right: 3%;
    }
    .content_9 {
      float: left;
      background: #f1f1f1;
      height: 434px;
      width: 439px;
      .content_10 {
        width: 50%;
        height: 50%;
        float: left;
        // background: red;
        padding-top: 6%;
        padding-left: 3%;

        .content_11 {
          font-size: 18px;
          font-family: PingFang-SC-Bold;
          font-weight: bold;
          color: rgba(0, 0, 0, 1);
          display: block;
          margin-bottom: 7%;
        }
        .content_12 {
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(0, 0, 0, 1);
          margin-bottom: 2%;
        }
      }
    }
    .content_13 {
      padding-left: 3%;
      width: 293px;
      height: 97px;
      float: left;
      // background: red;
      .content_7 {
        margin-top: 8%;
      }
      .content_15 {
        margin-top: 8%;
        float: left;
        background: #f1f1f1;
        height: 434px;
        width: 292px;
        padding-top: 9%;
        padding-left: 10%;
        .content_12 {
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(0, 0, 0, 1);
          margin-bottom: 4%;
        }
      }
    }
    .content_16 {
      margin-top: 72%;
      .content_7 {
        margin-top: 3%;
      }
      .content_17 {
        float: left;
        margin-top: 12%;
        margin-left: -28%;
        background: #f1f1f1;
        height: 79px;
        width: 439px;

        .content_12 {
          display: block;
          float: left;
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(0, 0, 0, 1);
          margin-left: 5%;
          margin-right: 9%;

          margin-top: 6%;
        }
      }
    }

    .content_18 {
      // fl
      margin-top: 68%;
      // margin-left: 18%;
      .content_7 {
        margin-left: 4%;
        margin-top: 6%;
      }
      .content_19 {
        display: block;
        float: left;
        font-size: 24px;
        font-family: PingFang-SC-Bold;
        font-weight: bold;
        color: rgba(0, 0, 0, 1);
        margin-left: 6%;
        width: 290px;
      }
      .content_20 {
        float: left;
        width: 290px;
        margin-top: 12%;
        margin-left: -33%;
        background: #f1f1f1;
        height: 79px;
        width: 290px;

        .content_12 {
          display: block;
          float: left;
          font-size: 18px;
          font-family: PingFang-SC-Regular;
          font-weight: 400;
          color: rgba(0, 0, 0, 1);
          margin-left: 9%;
          margin-top: 8%;
        }
      }
    }

    .content_14 {
      width: 439px;
      height: 530px;
      float: left;
      margin-right: 3%;

      // background: red;
    }
  }

  .fx3 {
    width: 929px;
    float: left;
    padding-left: 3.5%;
    padding-top: 6%;
    height: 3350px;
    background: rgba(255, 252, 252, 1);
    box-shadow: 0px 2px 6px 0px rgba(173, 173, 173, 0.4);
    border-radius: 10px 10px 0px 0px;
    margin-bottom: 35px;
    .content_1 {
      width: 195px;
      // background: red;
      height: 40px;
      margin: 0 auto;
      margin-bottom: 6%;
    }
    .content_2 {
      display: block;
      width: 17.5px;
      height: 35px;
      float: left;
      // padding-top:2%;
      border: 3px solid #646061;
      border-right: none;
    }
    .content_3 {
      display: block;
      width: 17.5px;
      height: 35px;
      float: right;
      margin-top: -14.5%;
      // margin-left: 6.5%;
      // padding-top:2%;
      border: 3px solid #646061;
      border-left: none;
    }
    .content_4 {
      display: block;
      float: left;
      margin-left: 4%;
      margin-top: -4%;
      font-size: 24px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(38, 32, 34, 1);
    }
    .content_5 {
      display: block;
      float: left;
      margin-left: 15%;
      font-size: 12px;
      font-family: PingFang-SC-Regular;
      font-weight: 400;
      color: rgba(38, 32, 34, 1);
    }
    .content_6 {
      height: 790px;
      width: 100%;
      // background: red;
      padding-left: 2.5%;
      padding-top: 1%;
    }
    .content_7 {
      float: left;
      margin-right: 2%;
    }
    .content_8 {
      display: block;
      float: left;
      font-size: 18px;
      font-family: PingFang-SC-Medium;
      font-weight: 500;
      color: rgba(38, 32, 34, 1);
      margin-top: -0.5%;
      margin-bottom: 3%;
    }
    .content_9 {
      float: left;
      display: block;
      margin-left: 5%;
      width: 95%;
      height: 227px;
      // background: green;
      .content_10 {
        float: left;
        margin-right: 1%;
      }
      .content_11 {
        display: block;
        margin-top: 13%;
        margin-right: 5%;
        float: left;
      }
      .content_12 {
        font-size: 18px;
        font-family: PingFang-SC-Medium;
        font-weight: 500;
        color: rgba(38, 32, 34, 1);
        display: block;
        margin-top: 8%;
        //  margin-top: 50%;
        // float: left;
      }
      .content_13 {
        font-size: 16px;
        font-family: PingFang-SC-Regular;
        font-weight: 400;
        color: rgba(38, 32, 34, 1);
        line-height: 24px;
        display: block;
        margin-top: 2%;
        //  margin-top: 50%;
        float: left;
      }
      .content_14 {
        font-size: 18px;
        font-family: PingFang-SC-Medium;
        font-weight: 500;
        color: rgba(38, 32, 34, 1);
        display: block;
        // vertical-align: middle;
        margin-top: 85px;
        margin-bottom: 19px;
      }
      .content_15 {
        font-size: 16px;
        font-family: PingFang-SC-Regular;
        font-weight: 400;
        color: rgba(38, 32, 34, 1);
        line-height: 24px;
      }
      .content_16 {
        display: block;
        float: right;
        margin-top: -155px;
        margin-right: 80px;
      }
      .content_17 {
        float: right;
        margin-right: 1%;
        display: block;
        margin-top: -60px;
      }
    }
  }

  #DW {
    height: 2300px;
  }
  #FX {
    height: 5000px;
  }
  #XY{
    padding-top: 2%;
    .content_1{
      display: block;
      margin-left: 30%;
    }
    .content_2{
      display: block;
    width: 64%;
    text-align: center;
    margin-left: 20%;
    margin-top: 30px;
    font-size:18px;
    font-family:PingFang-SC-Medium;
    font-weight:500;
    color:rgba(38,32,34,1);
    }

  }
  #DL{
    padding-top: 2%;
    .content_1{
      .content_2{
        float: left;
        display: block;
        width: 940px;
        font-size:18px;
        font-family:PingFang-SC-Regular;
        font-weight:400;
        color:rgba(38,32,34,1);
        margin-bottom: 45px;
      }
    }
  }
}
</style>

