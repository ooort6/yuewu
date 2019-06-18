<template>
    <div class="headerBar">
        <div class="layout">
            <!-- <div class="logo"><h1 @click="$router.push({name: 'home'})">MEIZU</h1></div> -->
            <div class="logo"><img @click="$router.push({name: 'home'})" src="@/static/images/logo.png" alt="" ></div>
             <!-- <div class="zhuce"> -->
              <!-- <Button type="primary"  @click="$router.push({name:'regist'})">立即注册</Button> -->
            <!-- </div> -->
            <!-- <div class="person"> -->
              <!-- <span><Icon  type="md-person"/>
                <h2 v-if="hasLogin == undefined"  @click="$router.push({name:'login'})">登录</h2>
                <h2 v-else @click="logout">退出</h2>
              </span> -->
              <!-- <span  class="carIcon" @click="goToCart">
                <Badge :count="1" type="error" :offset="[20,-3]">
                  <Icon type="md-cart" />
                </Badge>
              </span> -->
            <!-- </div> -->
          
            <div class="nav">
               <Menu mode="horizontal" :theme="'light'" >
                    <MenuItem class="nav-item" name="home" :to="{name:'home'}" >
                        <!-- <Icon type="ios-paper" /> -->
                        主页
                    </MenuItem>
                   
                    <MenuItem class="nav-item" name="design" :to="{name:'design'}">
                    设计理念
                    
                    </MenuItem>
                    <MenuItem class="nav-item" name="control" :to="{name:'control'}">
                        <!-- <Icon type="ios-people" /> -->
                        控制系统
                    </MenuItem>
                    <MenuItem class="nav-item" name="display" :to="{name:'display'}">
                        <!-- <Icon type="ios-people" /> -->
                        展示技术 
                    </MenuItem>
                    <MenuItem class="nav-item" name="success" :to="{name:'success'}">
                        <!-- <Icon type="ios-people" /> -->
                     成功案例 
                    </MenuItem>
               
                
                </Menu>
            </div>
        </div>
    </div>
</template>
<script>
import {loginOut } from "@/api/user"; 
export default {
    name:'headerBar',
    data(){
      return{
        hasLogin:'',
      }
    },
    mounted(){
      this.hasLogin = localStorage.getItem('userId')
    },
    methods:{
      goToCart(){
        this.$router.push({name:"cart"})
      },
      async logout(){
        const res = await loginOut()  
        if(res.status == 0){
          localStorage.clear()
          this.$router.push({name:'login'})
        }
      }
    }
}
</script>
<style lang="scss" scoped>
.headerBar{
    width: 100%;
    background: #fff;
    position:fixed;
    border-bottom: 1px solid #eee;
    z-index: 999;
    box-sizing: border-box;
box-shadow:0px 5px 5px 0px rgba(200,200,200,0.4);

    .layout{
        overflow: hidden;
        width: 1240px;
        margin: 0 300px;
          height: 69px;
        .logo{
          height: 57px;
          float: left;
          line-height: 57px;
          margin-top: 0.8%;
          margin-right:11%;
          img{
            height: 57px;
            width: 195px;
            // margin-left: 100px;
            display: block;
            &:hover{
            transition: all 0.8s linear;
            // cursor: pointer;
            }
          }
          h1{
            font-size: 40px;
            letter-spacing: 1px;
            color:#2d8cf0;
            &:hover{
              color:#333;
              transition: all 0.8s linear;
              cursor: pointer;
            }
          }
        }
        .person{
          float: right;
          height: 57px;
          font-size: 24px;
          line-height: 57px;
          width: 85px;
          .carIcon:hover{
            color: #2d8cf0;
            cursor: pointer;
          }
          h2{
            display: inline-block;
            font-size: 14px;
            color:#333;
            margin-right:30px;
            &:hover{
              cursor: pointer;
              color: #2d8cf0;
            }
          }
        }
        .zhuce{
          float: right;
          height: 57px;
          font-size: 24px;
          line-height: 57px;
          width: 120px;
        }
        .nav{
          margin-left: 10%;
          float: left;
          height: 57px; 
        }
       .ivu-menu-horizontal{
        // background: red;
        border: none;
        }
        // .ivu-menu .ivu-menu-light .ivu-menu-horizontal{
        //   background: red;
        // }

        .ivu-menu-horizontal.ivu-menu-light:after{
          background: none;
        }
        .nav-item{
          color: #262022;
          float: left;
          display: block;
          margin-right: 13px;
          font-size: 18px;
          font-family: PingFang-SC-Medium;
          margin-top:1%;
          border: none;
            margin-right: 52px;

        }
        .nav-item1{
           display: block;
            margin-right: 50px;
        }
      //  .ivu-menu-light.ivu-menu-horizontal .ivu-menu-item-active, .ivu-menu-light.ivu-menu-horizontal .ivu-menu-item:hover, .ivu-menu-light.ivu-menu-horizontal .ivu-menu-submenu-active, .ivu-menu-light.ivu-menu-horizontal .ivu-menu-submenu:hover{
      //     // color: #262022;
      //       border-bottom:#ff9900; 
      //       color: #ff9900;
      //   }
          .nav-item .ivu-menu-item .ivu-menu-item-active .ivu-menu-item-selected{
          border-bottom:none;

      }
      .ivu-menu-light.ivu-menu-horizontal .ivu-menu-item-active, .ivu-menu-light.ivu-menu-horizontal .ivu-menu-item:hover, .ivu-menu-light.ivu-menu-horizontal .ivu-menu-submenu-active, .ivu-menu-light.ivu-menu-horizontal .ivu-menu-submenu:hover{
          color: #ff9900;
          border-bottom:1px solid #ff9900; 

      }
  
    }
}
</style>

