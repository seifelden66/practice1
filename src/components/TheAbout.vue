<template>
  <div class="whole">
    <div class="halfLeft"></div>
    <div class="halfRight"></div>
    <div class="cont">
      <div class="image">
        <img src="../assets/proyecto 1-02.png" alt="das" />
      </div>
      <div class="text">
        <div class="title">
          <h1>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. At, inventore?
          </h1>
        </div>
        <div class="border"></div>
        <div class="desc">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum sit ea rerum
            iusto quis repudiandae autem, explicabo et! Temporibus, exercitationem esse
            alias amet laborum quaerat!
          </p>
        </div>
        <button>
          <h5>learn more</h5>
        </button>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.whole {
  position: relative;
  min-height: 80vh;
  display: flex;
  align-items: center;
  .halfLeft {
    top: -75px;
    left: 0;
    position: absolute;
    background: #ff5983;
    width: 100px;
    height: 200px;
    border-bottom-right-radius: 100px;
    border-top-right-radius: 100px;
    @media (max-width: 768px) {
      display: none;
    }
  }
  .halfRight {
    @media (max-width: 768px) {
      display: none;
    }
    bottom: 0;
    right: 0;
    position: absolute;
    background: #ff5983;
    width: 100px;
    z-index: -1;
    height: 200px;
    border-bottom-left-radius: 100px;
    border-top-left-radius: 100px;
  }
  .cont {
    @media (max-width: 768px) {
      margin-top: 7em;
      grid-template-columns: 1fr;
      place-items: center;
      text-align: center;
    }
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    button {
      border: none;
      background: #303030;
      color: white;
      padding: 10px;
      border-radius: 5px;
      margin-top: 1em;
      cursor: pointer;
      transition: 300ms;
      &:hover {
        background: #046c6a;
      }
    }
    .image {
      @media (max-width: 768px) {
        display: none;
      }
      width: 400px;
    }
    .text {
      @media (max-width:768px) {
        display: flex;
        flex-direction: column;
        align-items: center;
      }
      .title {
        h1 {
          color: #ff5983;
        }
      }
      .border {
        background: #000;
      }
    }
  }
}
</style>
