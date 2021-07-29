<template >
  <div id="app">
    <b-navbar toggleable="sm" type="white" variant="">
      <b-navbar-brand href="#">
        <router-link to="/"><img class="logoimg" src="@/assets/diarylogotrans.png" alt="Kitten"></router-link>
      </b-navbar-brand>
      <b-nav-text><router-link to="/about" class="navtext">로그인</router-link></b-nav-text>
    </b-navbar>
    <router-view/>
  </div>
</template>



<style>

@import url('https://fonts.googleapis.com/css2?family=Gowun+Batang&display=swap%27');

.logoimg{
  height:40px;
  width:40px;
  object-fit: scale-down;
}
.navtext{
  font-family: 'Gowun Batang', serif;
  font-size: 15px;
  color:#B1B1B1;
  text-decoration:none;
}

.navtext:hover{
  color:#B1B1B1;
  text-decoration:none;
}
#body{
  color: #B2B8A3;
  background-color: #000000;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
