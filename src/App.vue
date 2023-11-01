<script setup>

</script>

<template>
<div class="wrapper">
  <div class="profile">

    <div class="ballon">12</div>
  </div>

  <div class="buttomw">
   <div class="buttom" >
    <div>-</div>
   </div>
   <div class="buttom" >
    <div>+</div>
   </div>
  </div>
</div>

</template>

<style scoped>

.wrapper{
 background-color: #FF6B1A;
 width: 60%;
 padding-top: 18px;
 border-radius: 12px;
 margin: 0 auto;
 
}
.profile{
  
  height: 200px;
  width: 200px;
  margin: auto;
  border-radius: 100%;
  margin-top: 40px;
  position: relative;
  background-image: url("https://ets2.lt/wp-content/uploads/2018/09/Profile-Photo-Square.jpg");
  background-size: cover;
  }
  .ballon{
    width: 32px;
    height: 32px;
    background-color: red;
    border-radius: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    position: absolute;
    top: 0px;
    right: 0px;
    
  }
  .buttom{
    background-color: rgb(253, 248, 249);
    display: inline-block;
    border-radius: 4px;
    width: 32px;
    margin: 0 8px;
    padding: 4px 0;
 
 
  }
  .buttomw{
   
    overflow: hidden;
   
    text-align: center;
    margin-top: 16px;
    margin-bottom: 16px;
    
  }

  
  
</style>
