<template>
  <div class="success">
        <div class="success_1">
            <div style="margin:0 auto;width:1080px">
  <div class="success_2"></div>
<div class="success_2"></div>
<div class="success_2"></div>
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
            .success_2{
                width:319px;
                height:319px;
                background:rgba(250,251,253,1);
                box-shadow:0px 10px 10px 1px rgba(173,173,173,0.3);
                float: left;
                display: block;
                margin: 0 auto;
                margin-right: 41px;


            }
        }
  }
</style>

