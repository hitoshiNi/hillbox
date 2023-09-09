<template>
  <div class="container">
    <div class="header">
      <div class="menu">
        <div class="button_before"><button v-on:click="open" ><img src="../assets/sozai_cman_jp_20200722022512.png" class="sansen"></button></div>
        <div class="box"><img src="../assets/icon.PNG" class="icon"></div>
        <div class="hidden" v-show="isopen">
          <button v-on:click="close" class="button_after"><img src="../assets/batsu.svg" class="batsu"></button>
          <div class="menu_details">
            <p><button v-on:click="close"><router-link to="/">▷HILLBOX inc. TOP</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/company">▷会社概要</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/">▷マーケティング・PR企画</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/">▷インバウンド/グローバル</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/">▷システム開発/デジタル広告</router-link></button></p>
            <pre><button v-on:click="close"><a href="https://twistantwin.com/">    ▶TwistanWin</a></button></pre>
            <p><button v-on:click="close"><router-link to="/privacy">▷Privacy policy</router-link></button></p>
          </div>
        </div>
      </div>
    </div>
    <img src="../assets/main_logo.PNG" class="main_logo">
    
    <div class="contents">
      <div class="content">
        <div class="robo_maru">
          <img src="../assets/robotR.png" class="robo">
        </div>
       <section class="detail_box">
         <div class="detail">
          <h1>マーケティング・PR企画</h1>
          <p>〇課題抽出から、コンセプト設計、商品企画、PRまでトータルに提案実施
            <br>〇CM、グラフィック、各種動画制作
            <br>〇異業種コラボ、新タッチポイント創出</p>
         </div>
       </section>
      </div>
      <div class="content">
        <div class="robo_maru">
          <img src="../assets/robotG.png" class="robo">
        </div>
       <section class="detail_box">
         <div class="detail">
          <h1>インバウンド/グローバル</h1>
          <p>〇⽵内亮はじめKOL、KOC施策。⽇中、北東亜マーケの推進
            <br>〇微博、微信、各種SNS運⽤
            <br>○富裕層マーケ、チャネル開拓</p>
         </div>
       </section>
      </div>
      <div class="content">
        <div class="robo_maru">
          <img src="../assets/robotY.png" class="robo">
        </div>
       <section class="detail_box">
         <div class="detail">
          <h1>システム開発/デジタル広告</h1>
          <p>〇システム開発と広告運⽤を融合
            <br>〇各種SNS、ECサイト開設運営
            <br><a href="https://twistantwin.com/">〇＠HILLBOX製 TwistantWin</a></p>
          
         </div>
       </section>
      </div>
    </div>  
    <div class="links">
        <router-link to="/privacy" class="link_to_privacy"> ▷Privacy policy</router-link>
        <router-link to="/company" class="link_to_company"> ▷HILLBOX inc.</router-link>
    </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      isopen: false,
    }
  },
  methods: {
    open: function(){
      this.isopen = true;
      console.log(this.isopen);
    },
    close: function(){
      this.isopen = false;
    }
    }
  }

</script>

<style>
@import "../assets/design.css";
</style>


