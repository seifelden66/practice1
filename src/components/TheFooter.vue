<template>
  <div class="cont">
    <div class="left">
      <h1>UXTIFY</h1>
      <div class="cencen">
        <div>
          <p>about</p>
        </div>
        <div>
          <p>prices</p>
        </div>
        <div>
          <p>contact</p>
        </div>
        <div>
          <p>services</p>
        </div>
      </div>
      <div class="btt">
        <p>UXTIFY2019 - by Lorem, ipsum.</p>
      </div>
    </div>
    
    <div class="center">
      <div class="line">
        <div class="icon">
          <Location />
        </div>
        <p>Caracas - venezuela</p>
      </div>
      <div class="line">
        <div class="icon">
          <Phone />
        </div>
        <p>445645411514894</p>
      </div>
      <div class="line">
        <div class="icon">
          <Location />
        </div>
        <p>nlnlkn</p>
      </div>
    </div>
    
    <div class="right">
      <h1>hello</h1>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ducimus fugiat, neque minus aut perferendis aperiam?</p>
    </div>
  </div>
</template>

<script setup>
import Location from "./icons/Location.vue";
import Phone from "./icons/Phone.vue";
</script>

<style lang="scss" scoped>
.line {
  display: flex;
  align-items: center;
  gap: 5px;
  .icon{
    color: #ff5983;
  }
}
.cont {
    @media (max-width: 768px) {
        display: grid;
        grid-template-columns: 1fr;
        place-items: center;
        text-align: center;
        
      }
  margin-top: 1em;
  margin-bottom: 1em;
  display: flex;
  justify-content: space-between;
  align-items: center;
  .left {
    
    .cencen {
      color: rgb(40, 38, 56);
      display: flex;
      gap: 1.3em;
      align-items: center;
      @media (max-width: 768px) {
        gap: .6em;
        flex-wrap: wrap;
        
      }
      
    }
    .btt {
      color: #ff5983;
    }
  }
  .center{
    line-height: 45px;
    @media (max-width: 768px) {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        line-height:normal
        
      }
  }
  .right{
    width: 20%;
    h1{
        color: #ff5983;
    }
    @media (max-width: 768px) {
        width: 80%;
    }
  }
}
</style>
