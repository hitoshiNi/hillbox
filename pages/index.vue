<template>
  <div class="container">
    <div class="header">
      <div class="menu">
        <div class="button_before"><button v-on:click="open" ><img src="../assets/≡.svg" class="sansen"></button></div>
        <div class="box"><img src="../assets/icon.PNG" class="icon"></div>
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
          <p>〇デジタルマーケティング全般の戦略策定・導入支援・運用コンサルティング
            <br>〇リスティング・動画広告・SNS広告などを活用したマーケティング施策</p>
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


