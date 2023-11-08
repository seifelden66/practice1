<template>
  <div class="hh">
    <div class="cont">
      <nav class="nav">
        <div class="left">
          <h1>UXTIFY</h1>
        </div>
        <div @click="open" class="menu"  v-if="!isOpen">
          <Menu />
        </div>
        <div @click="open" class="menu"  v-else>
          <Close />
        </div>
        <div v-show="isOpen" class="bb">
            <Sidebar />
        </div>

        <div class="center">
          <div class="cencen">
            <div>
              <h2>about</h2>
            </div>
            <div>
              <h2>prices</h2>
            </div>
            <div>
              <h2>contact</h2>
            </div>
            <div>
              <h2>services</h2>
            </div>
          </div>
        </div>

        <div class="right">
          <div class="btn">
            <h5>CLICK</h5>
            
          </div>
        </div>
        <div class="shape"></div>
      </nav>
    </div>
  </div>
</template>

<script setup>
import Menu from './icons/Menu.vue';
import Close from './icons/Close.vue';
import { ref } from 'vue';
import Sidebar from './Sidebar.vue';
const isOpen = ref(false)
const open = ()=>{
    isOpen.value = !isOpen.value
}

</script>

<style scoped lang="scss">
.hh {
  position: relative;
  .bb{
    position: absolute;
    top: 20%;
    right: 7%;
    transition: 300ms;
  }
  .nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 2em;
    .left {
      h1 {
        font-weight: 300;
      }
    }
    .menu {
    
      cursor: pointer;
      @media (min-width:992px) {
        display: none;
      }
    }
    .center {
      .cencen {
        color: rgb(40, 38, 56);
        display: flex;
        gap: 1.3em;
        align-items: center;
      }
      @media (max-width: 992px) {
        display: none;
      }
    }
    .right {
      @media (max-width: 992px) {
        display: none;
      }
      z-index: 1;
      .btn {
        padding: 1em;
        background: #ffffff;
        display: flex;
        align-items: center;
        justify-content: center;
        height: 10px;
        width: 80px;
        border-radius: 5px;
        transition: 300ms;
        cursor: pointer;
        color: #ff5983;
        &:hover {
          background: rgb(255, 210, 47);
        }
      }
    }
    .shape {
      @media (max-width: 768px) {
        display: none;
      }
      position: absolute;
      background: #ff5983;
      top: 0;
      right: 0;
      width: 295px;
      height: 350px;
      border-top-left-radius: 15%;
      border-bottom-left-radius: 90%;
      z-index: 0;
    }
  }
}
</style>
