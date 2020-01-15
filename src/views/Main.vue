<template>
<div class="main">
  <Navbar />

  <div class="container">
    <div class="content">
      <div class="logo">
        <img src="@/assets/img/logo.png" alt="logo">
      </div>

      <input type="text" placeholder="Buscar Invocador ou Campeão">

      <div class="download_windows">
        <button> <img src="@/assets/img/windows.png" alt="image-windows"><span>Baixar grátis para Windows</span></button>
      </div>

      <div class="container_video">
        <img src="@/assets/img/play.png" alt=""><span class="video">Executar vídeo</span>
      </div>

      <br><br><br>

      <div class="container__games">
        <div class="league_of_legends">
          <img src="@/assets/img/lol.png" alt="lol-img">
        </div>
        <div class="teamfight_tactics">
          <img src="@/assets/img/tft.png" alt="lol-img" style="margin-left: 10px;">
        </div>
        <div class="legends_of_runeterra">
          <img src="@/assets/img/runeterra.png" alt="lol-img" style="margin-left: 10px;">
        </div>
      </div>
      
    </div>
  </div>
</div>
</template>

<script>
import Navbar from '@/components/Navbar';

export default {
  name: "main",
  components: {
    Navbar
  }
}
</script>

<style lang="scss">
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 80vh;

    .content {
      height: 500px;
      width: 650px;

      .logo {
        display: flex;
        justify-content: center;
      }

      input {
        margin-top: 50px;
        width: 610px;
        padding: 20px;
        background-color: #222C3F;
        border: 1px solid #48546B;
        border-radius: 7px;
      }
      ::-webkit-input-placeholder {
        font-size: 16px;
        color: #8399AE; 
      }

      .download_windows {
        margin-top: 25px;
        display: flex;
        justify-content: center;
        button {
          display: flex;
          padding: 10px 30px;
          background-color: #FF5859;
          font-size: 14px;
          font-weight: bold;
          cursor: pointer;
          color: #FFF;
          border: 0;
          border-radius: 5px;

          span {margin: 3px 10px; }
        }
        :hover { background-color: #FF7B7D; }
      }

      .container_video {
        margin-top: 10px;
        display: flex;
        justify-content: center;

        .video {
          display: block;
          text-align: center;
          font-size: 12px;
          color: #BBC9E0;
        }
      }

      .container__games {
        display: flex;
        justify-content: center;
      }
    }
  }



</style>