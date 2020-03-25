<template>
  <div class="container">
    <div class="header">
    <div class="menu">
      <button v-on:click="open" class="button" >menu</button>
      <div class="hidden" v-show="isopen">
        <button v-on:click="close" class="button">×</button>
        <p><router-link to="/company">▷HILLBOX inc.</router-link></p>
        <p><router-link to="/company">▷会社概要</router-link></p>
        <p><router-link to="/">▷マーケティング・PR企画</router-link></p>
        <p><router-link to="/">▷デジタルマーケティング</router-link></p>
        <p><router-link to="/">▷アプリ/WEBサービス開発</router-link></p>
        <p><router-link to="/privacy" class="link_to_privacy">▷Privacy policy</router-link></p>
      </div>
    </div>
    <img src="../assets/icon.png" class="icon">
    </div>
    <img src="../assets/main_logo.png" class="main_logo">
    
    <div class="contents">
      <div class="content">
        <img src="../assets/robotY.png" class="robo">
       <section class="detail">
         <h1>マーケティング・PR企画</h1>
         <p>〇課題抽出から、コンセプト設計、商品企画、コミュニケーション提案の実行まで</p>
         <p>〇マス広告、イベント、SNS広告、PRなど</p>
       </section>
      </div>
       <div class="content">
         <img src="../assets/robotR.png" class="robo">
       <section class="detail">
         <h1>デジタルマーケティング</h1>
         <p>〇LINEなどを活用したマーケティング施策のコンサルティングから開発、実行</p>
         <p>〇公式アカウント、LINE BOT、運用広告など</p>
       </section>
       </div>
       <div class="content">
         <img src="../assets/robotG.png" class="robo">
       <section class="detail">
         <h1>アプリ/WEBサービス開発</h1>
         <p>〇アプリやWEBサービス、ITシステムの企画から開発まで</p>
         <p>〇新規サービス、業務効率化、ECサイトなど</p>
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


