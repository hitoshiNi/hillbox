<template>
  <div class="container">
    <div class="header">
      <div class="menu">
        <button v-on:click="open" class="button_before"><img src="../assets/≡.svg"></button>
        <div class="hidden" v-show="isopen">
          <button v-on:click="close" class="button_after">×</button>
          <div class="menu_details">
            <p><button v-on:click="close"><router-link to="/">▷HILLBOX inc. TOP</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/company">▷会社概要</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/">▷マーケティング・PR企画</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/">▷デジタルマーケティング</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/">▷アプリ/WEBサービス開発</router-link></button></p>
            <p><button v-on:click="close"><router-link to="/privacy">▷Privacy policy</router-link></button></p>
          </div>
        </div>
      </div>
      <img src="../assets/icon.png" class="icon">
    </div>
    <img src="../assets/main_logo.png" class="main_logo">
    
    <div class="contents">
      <div class="content">
        <div class="robo_maru">
          <img src="../assets/robotR.png" class="robo">
        </div>
       <section class="detail_box">
         <div class="detail">
          <h1>マーケティング・PR企画</h1>
          <p>〇課題抽出から、コンセプト設計、商品企画、コミュニケーション提案の実行まで
            <br>〇マス広告、イベント、SNS広告、PRなど</p>
         </div>
       </section>
      </div>
      <div class="content">
        <div class="robo_maru">
          <img src="../assets/robotG.png" class="robo">
        </div>
       <section class="detail_box">
         <div class="detail">
          <h1>デジタルマーケティング</h1>
          <p>〇LINEなどを活用したマーケティング施策のコンサルティングから開発、実行
            <br>〇公式アカウント、LINE BOT、運用広告など</p>
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
            <br>〇新規サービス、業務効率化、ECサイトなど</p>
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


