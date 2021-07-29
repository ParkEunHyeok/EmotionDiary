<template>
    <div class="bg">
        <h1 class="writediaryfont"> 일기 쓰기 </h1>
        <center>
        <b-form-textarea
            id="textarea"
            v-model="text"
            placeholder=""
            rows="20"
            max-rows="20"
            class="inputtext"
    ></b-form-textarea>
        <div v-if="showresult == true">
            <img src="../assets/moong.png" class="aiimg">
        </div>
        <b-button pill class="submitbutton"> <b>Enter</b> </b-button>
        </center>
    </div>    
</template>
<script>
export default {
    data() {
        return {
            showresult : true,
        }
    },
}
</script>
<style scoped>
.aiimg{
    float:left;
    margin-left:5vh;
    margin-top : 3vh;
    height:80px;
    width:80px;
}
.bg{
    height:100%;
    background-color: #FFF5EB;
}
.writediaryfont{
    font-family: 'Gowun Batang', serif;
  font-size: 5vh;
  padding-top: 5vh;
    padding-left:calc(10vw + env(safe-area-inset-left));
  padding-right:calc(10vw + env(safe-area-inset-right));
  text-align: left;
}
.inputtext{
    align-content:center;
    width:80%;
    border-radius:25px;
    background-color: white;
    margin-top : 3vh;
}
.submitbutton{
  font-family: 'Gowun Batang', serif;
  font-size: 4vh;
  height:7vh;
  width:80%;
  margin-top:5vh;
  margin-bottom: 5vh;
  background-color: #000000;
  border:0;

}
</style>