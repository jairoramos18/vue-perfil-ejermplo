<script setup>
import { ref } from 'vue';

let qty = ref (0)
function addvalue(){
  qty.value ++
  console.log(qty)
}
function minusvalue(){
  
  if (qty.value>0){
    qty.value--
    
  }
  console.log(qty)
 
}
</script>

<template>
<div class="wrapper">
  <div class="profile">

    <div class="ballon" v-show="qty>0">{{ qty }}</div>
  </div>

  <div class="buttomw">
   <div class="buttom"  @click="minusvalue"><div>-</div>
   </div>
   <div class="buttom" @click="addvalue">  <div>+</div>
   </div>
  </div>
  <div v-if="qty">me escribieron 😂 </div>
  <div v-else >nadie me escribe 😒</div>
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
