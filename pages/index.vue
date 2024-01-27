<template>
  <div class="container">

    <img src="../assets/main_logo.PNG" class="main_logo">
    
    <div class="contents">
       <div class="content">
        <div class="robo_maru">
          <img src="../assets/robotY.png" class="robo">
        </div>
       <section class="detail_box">
         <div class="detail">
          <h1>ホームページは移転しました。</h1>
          <p>
            <br><a href="http://hillbox.net/">〇移転先リンク</a>
            <br>
            <br><a href="https://twistantwin.com/">〇＠HILLBOX製 TwistantWin</a></p>
          
         </div>
       </section>
      </div>

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


