<template>
    <div class="login" id="login-app">
      <div class="login-box">


        <div class="block text-center zoumadeng" style="margin-right: 3px">
          <el-carousel height="474.38px" style="border-radius: 12px">
            <el-carousel-item v-for="item in arrImg" :key="item">
              <!--            <h3 class="small justify-center" text="2xl">{{ item }}</h3>-->
              <!--            <img src="@/images/Tips{{item}}.jpg" alt="" style="height: 474.38px">-->
              <el-image :src="item" style="height: 474.38px">

              </el-image>
            </el-carousel-item>
          </el-carousel>
        </div>

        <div class="login-form" style="position: relative;">
            <div class="fanhuidenglu">
              <img src="../images/tips2.png" alt="" style="width:200px; position: absolute; top: 15px; right: 55px;">
              <img src="../images/erweima.png" alt=""
              style="width: 50px; height: 50px;  position: absolute; top: 2px; right: 2px;"
              @click="fanhui"
              >
            </div>
          <img src="../images/image-removebg-preview.png" alt="" >
        </div>
      </div>
  
    </div>
  
  </template>
  
  <script>
 
  export default {

    data() {
      return {
        arrImg:[
          //动态添加数据是require
          require("../images/Tips1.jpg"),
          require("../images/Tips2.jpg"),
          require("../images/Tips3.jpg"),
          require("../images/Tips4.jpg")
        ]
      }
    },
    methods: {
      fanhui(){
        this.$router.push('/')
      },
    }
  };
  </script>
  
  
  <style scoped>
  @import "@/styles/erweima.css";
    
  </style>
  