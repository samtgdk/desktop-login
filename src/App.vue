<template>
  <div class="main">
    <div class="left">
   <div class="container">
    <div class="top">
          <img class="top-img" src="./components/img/Cursive Italic Multipurpse Typography Logo Design Brand Identity Clean Comic Style for Design Company 1.png" alt="">

    </div>
    
    <h1>Log In</h1>
   <input class="title" type="text" placeholder="email id" id="mail" v-model="email">
   <input class="title" type="password" placeholder="password" id="pass" v-model="pass">
   <div class="bottom">
    <input type="checkbox" id="remember">
    <label for="remember" class="title">Remember me</label>
    <p class="title"><a href="#">Forgot password</a> </p>
   </div>
   <input class="button" type="submit" value="Log In" @click="validate()">
    <span class="with-line">or</span>
    <div class="rounds">
      <div class="round-left">
        <img class="picture" src="./components/img/indir.png" alt="">
      </div>
      <div class="round-right">
        <img class="picture" src="./components/img/Twitter_icon-icons.com_66803.png" alt="">
      </div>
    </div>
  </div>
    
  </div>
  <div class="right">
    <img class="bigPic" src="./components/img/Screenshot_1.png" alt="">
  </div>
  </div>
  
</template>
<script setup>
import "./components/img/SCSS/main.css";
</script>
<script>
export default {
  methods: {
      validate(){
      let username = this.email
      let pass = this.pass

      if (username == 'login123' && pass == 123456) {
        alert("Login Successfuly");
      }else{
        alert("Try Again");
      }
    }
  },
}
</script>

<style>

</style>