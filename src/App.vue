<template>
  <div class="main">
    <div class="left">
   <div class="container">
    <div class="top">
          <img class="top-img" src="./assets/img/write.png" alt="">

    </div>
    
    <h1>Log In</h1>
   <input class="title" type="text" placeholder="email id" id="mail" v-model="email">
   <input class="title" type="password" placeholder="password" id="pass" v-model="pass">
   <div class="bottom">
    <div class="check">
      <input type="checkbox" id="remember">
      <label for="remember" class="title">Remember me</label>
    </div>
    <p class="title"><a href="#">Forgot password</a> </p>
   </div>
   <button class="submit-button" type="submit" value="Log In" @click="validate()">Log In</button>
   
    <div class="rounds">
      <div class="round-left">
        <img class="picture" src="./assets/img/indir.png" alt="">
      </div>
      <div class="round-right">
        <img class="picture" src="./assets/img/Twitter_icon-icons.com_66803.png" alt="">
      </div>
    </div>
  </div>
    
  </div>
  <div class="right">
    <img class="bigPic" src="./assets/img/Screenshot_1.png" alt="">
  </div>
  </div>
  
</template>
<script setup>
import "./assets/SCSS/main.css";
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
#app{
  display: flex;
  justify-content: center;
  margin-top: 20px;
}
</style>