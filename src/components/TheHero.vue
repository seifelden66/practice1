<template>
<div class="main">
  <div class="cont">
    <div class="ccont">
      <div class="text">
        <div class="title">
          <h1>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Placeat, earum.
          </h1>
        </div>
        <div class="border"></div>
        <div class="desc">
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Enim nesciunt ipsam
            quibusdam excepturi corporis, voluptatem eum consequuntur dolor et nam quod?
            Facere eveniet voluptas beatae fugit tenetur assumenda voluptatum mollitia
            porro ut asperiores Lorem ipsum dolor, sit amet consectetur adipisicing elit.
            Odio, consequuntur?
          </p>
        </div>
        <button>submit</button>
      </div>
      <div class="image">
        <img src="../assets/parte 1.png" alt="hh" />
      </div>
    </div>
  </div>
</div>
</template>

<script setup></script>

<style lang="scss" scoped>
.cont {
  .ccont {
    @media (max-width: 768px) {
      padding-top: 10em;
        grid-template-columns: 1fr;
        place-items: center;
        text-align: center;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        height: 50vh;
      }
    height: 70vh;
    display: grid;
    align-items: center;
    grid-template-columns: 1fr 1fr;
    gap: 2em;
    .text {
      @media (max-width: 768px) {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
      }
     
      button{
        background: #08d9d6;
        color: white;
        border: none;
        padding: 10px;
        margin-top: 5px;
        width: 100px;
        border-radius: 5px;
        transition: 300ms;
        cursor: pointer;
        &:hover{
            background: #046c6a;
        }
      }
    }
    .image {
      
      z-index: 2;
      img {
        width: 100%;
      }
    }
  }
}
</style>
