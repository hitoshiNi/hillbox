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
      <img src="../assets/icon.PNG" class="icon">
    </div>
    
    <img src="../assets/main_logo.PNG" class="main_logo">
    
    <div class="contents">
      <div class="content">
        <div class="robo_maru">
          <img src="../assets/building.png" class="robo">
        </div>
       <section class="detail_box">
        <div class="detail">
          <h1>会社概要</h1>
          <pre>社名 ：ヒルボックス株式会社<br>     HILLBOX inc.<br>所在地：〒153-0061<br>     東京都目黒区中目黒5-28-18-202</pre>
          <p>代表取締役：岡友紀</p>
          <p>問い合わせ：info@hillbox.net</p>
        </div>
       </section>
       </div>

    </div>  
    <div class="links">
       <router-link to="/privacy" class="link_to_privacy"> ▷Privacy policy</router-link>

    </div>
    </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo,
  },
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
};


</script>

<style>
@import "../assets/design.css";
</style>


