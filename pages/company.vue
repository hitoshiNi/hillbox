<template>
  <div class="container">
    <div class="header">
    <img src="../assets/icon.png" class="icon">
    </div>
    <img src="../assets/main_logo.png" class="main_logo">
    
    <div class="contents">
      <div class="content">
       <section class="detail">
         <h1>会社概要</h1>
         <pre>社名：ヒルボックス株式会社<br>     HILLBOX inc.</pre>
         <pre>所在地：〒153-0061<br>      東京都目黒区中目黒5-28-18-202</pre>
         <p>代表取締役：岡友紀</p>
         <p>問い合わせ：info@hillbox.net</p>
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
  }
};
</script>

<style>
@import "../assets/design.css";
</style>


