<template>
  <div class="whole">
    <div class="cont">
      <div class="center">
        <h1>Lorem ipsum dolor</h1>
        <h4>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Explicabo amet.</h4>
        <button>
          <h5>learn More</h5>
        </button>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.whole {
  margin-top: 2em;
  background-image: url("../assets/proyecto\ 1-03.png");
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
  min-height: 50vh;
 
  .cont {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 50vh;

    .center {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      width: 40%;
      color: white;
      text-align: center;
      @media (max-width: 768px) {
        width: 80%;
  }
      button {
        background: #00f8cf;
        border: none;
        color: white;
        padding: 10px;
        border-radius: 5px;
        margin-top: 1em;
        cursor: pointer;
        transition: 300ms;
        &:hover{
            background: #046c6a;
        }
      }
      h1 {
        font-weight: 700;
      }
    }
  }
}
</style>
