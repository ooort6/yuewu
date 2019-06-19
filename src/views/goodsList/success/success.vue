<template>
  <div class="success">
        <div class="success_1">
            <div style="margin:0 auto;width:1269px">
              <div class="triangle_border_left">
</div>
                                                      
<!-- 向右的三角形 -->

  <div class="success_2">
    <img class="success_3" src="../../../static/images/anli1.png" alt="">
    <span class="success_4">上海电信客户体验中心</span>
    <Button class="success_5" @click="$router.push({name: 'success_sh'})">点击详情</Button>
  </div>
<div class="success_2">
    <img class="success_3" src="../../../static/images/anli2.png" alt="">
    <span class="success_4">云南移动综合体验厅</span>
    <Button class="success_5" @click="$router.push({name: 'success_yn'})">点击详情</Button>
</div>
<div class="success_2">
    <img class="success_3" src="../../../static/images/anli3.png" alt="">
    <span class="success_4">天津电信信息化体验厅</span>
    <Button class="success_5" @click="$router.push({name: 'success_tj'})">点击详情</Button>
</div>
<div class="triangle_border_right">
</div>
            </div>
              
        </div>
    
  </div>
</template>
<script>
export default {
    name:'success',
    data() {
    return {
     
    };
  },
  mounted(){

  },

}
</script>
<style lang="scss" scoped>
  .success{
       padding-top: 5%;
       height: 100%;
       background: url('../../../static/images/anli.jpg') ;
        // width: 200px;
        // background: red;
        .success_1{
            height: 320px;
            width: 100%;
            // background: red;
            margin-top: 140px;
            .triangle_border_left{
    width:0;
    height:0;
    border-width:30px 30px 30px 0;
    border-style:solid;
    border-color:transparent #CFCFCF transparent transparent;/*透明 灰 透明 透明 */
    // margin:40px auto;
    // position:relative;
    float: left;
    margin-right: 85px;
    margin-top: 10%;
    cursor: pointer;
}

/*向右*/
.triangle_border_right{
    width:0;
    height:0;
    border-width:30px 0 30px 30px;
    border-style:solid;
    border-color:transparent transparent transparent #CFCFCF;/*透明 透明 透明 灰*/
    // margin:40px auto;
    // position:relative;
     float: left;
     margin-left: 44px;
    margin-top: 10%;
    cursor: pointer;

}

            .success_2{
                width:319px;
                height:319px;
                background:rgba(250,251,253,1);
                box-shadow:0px 10px 10px 1px rgba(173,173,173,0.3);
                float: left;
                display: block;
                margin: 0 auto;
                margin-right: 41px;
              .success_3{
                
                display: block;
                margin: 0 auto;
                margin-top: 29px;
              }
              .success_4{
                display: block;
                text-align: center;
                font-size:24px;
                font-family:PingFang-SC-Medium;
                font-weight:500;
                color:rgba(38,32,34,1);
                margin-bottom: 11px;
              }
              .success_5{
                display: block;
                margin: 0 auto;
                width:249px;
                height:30px;
                background:rgba(255,199,56,1);
                color: #fff;
              }

            }
        }
  }
</style>

