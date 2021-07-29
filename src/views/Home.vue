<template>
  <div class="Home">
    <div class="intro">
      <h1 class="introfont">한 줄 일기를 적고,<br> 인공지능에게 위로를 받아보세요🤗</h1>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  components: {

  }
}
</script>

<style scoped>

.intro{
  background-color:#FFF5EB;
  height:30vh;
  width:100%;
  text-align:left;
}
.introfont{
  font-family: 'Gowun Batang', serif;
  font-size: 2.5vh;
  padding-top:10vh;
  padding-left:calc(5vw + env(safe-area-inset-left));
  padding-right:calc(5vw + env(safe-area-inset-right));

}
</style>
