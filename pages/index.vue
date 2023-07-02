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
            <p><button v-on:click="close"><router-link to="/">▷財務経理コンサルティング</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/">▷人事労務業務コンサルティング</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/">▷アプリ/WEBサービス開発</router-link></button></p>
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
          <h1>財務経理コンサルティング</h1>
          <p>〇財務面から課題を抽出。適切な財務環境へアドバイス
            <br>〇経理は経営の羅針盤。適切な財務指標把握が経営の指針に
            <br>〇経理・経営コンサルティング</p>
         </div>
       </section>
      </div>
      <div class="content">
        <div class="robo_maru">
          <img src="../assets/robotG.png" class="robo">
        </div>
       <section class="detail_box">
         <div class="detail">
          <h1>人事労務業務コンサルティング</h1>
          <p>〇企業における採用から退職までの社会保険に関する諸問題や年金相談
            <br>〇人事労務管理を中心としたアドバイス</p>
         </div>
       </section>
      </div>
      <div class="content">
        <div class="robo_maru">
          <img src="../assets/robotY.png" class="robo">
        </div>
       <section class="detail_box">
         <div class="detail">
          <h1>アプリ/WEBサービス開発</h1>
          <p>〇アプリやWEBサービス、ITシステムの企画から開発まで
            <br>〇新規サービス、業務効率化、ECサイトなど
            <br><a href="https://twistantwin.com/">〇TwistantWin</a></p>
          
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


