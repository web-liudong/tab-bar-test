<template>
  <div id="app">
     
   <tab-bar>
      <tab-bar-item path="/home" activeColor="red">
  <img  slot="item-icon" src="./assets/img/message.png" alt="">
  <img  slot="item-icon-active" src="./assets/img/benefits.png" alt="">
        <div slot="item-text">首页</div>
      </tab-bar-item>
       <tab-bar-item path="/category" activeColor="red">
 <img  slot="item-icon" src="./assets/img/record.png" alt="">
 <img  slot="item-icon-active" src="./assets/img/down_to_bottom.png" alt="">
        <div slot="item-text">会员</div>
       </tab-bar-item>
        <tab-bar-item path="/cart" activeColor="red">
 <img  slot="item-icon" src="./assets/img/time.png" alt="">
 <img  slot="item-icon-active" src="./assets/img/social_github.png" alt="">
        <div slot="item-text">查询</div>
        </tab-bar-item>
         <tab-bar-item path="/profile" activeColor="red">
 <img  slot="item-icon" src="./assets/img/view.png" alt="">
 <img  slot="item-icon-active" src="./assets/img/up_to_top.png" alt="">
        <div slot="item-text">我的</div>
         </tab-bar-item>
   </tab-bar>

    <router-view></router-view>
 
  </div>
 
</template>

<script>
import TabBar from './components/tabbar/TabBar'
import TabBarItem from './components/tabbar/TabBarItem'
export default {
  name: 'App',
  components:{
    TabBar,
    TabBarItem
  }
}
</script>

<style>
    @import "./assets/css/base.css";
</style>
 