<template>
  <nav>
    <div class="leftSide">
      <div class="logoNavbar">
        <img src="@/assets/img/logo-navbar.png" alt="logo-navbar">
      </div>
      <span>Escolha um Jogo</span>
    </div>
    <div class="rightSide">
      <ul>
        <li>
          <a class="language" href="#">Português</a>
        </li>
        <li>
          <a class="logIn" href="#">Entrar</a>
        </li>
        <li>
          <a class="downloadApp" href="#">Baixe o App</a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 3px;
  background-color: #0e1726;

  .leftSide {
    display: flex;
    align-items: center;
    margin-left: 30px;

    span {
      margin-left: 50px;
      letter-spacing: 0.08em;
      font-size: 14px;
      color: #BBC9E0;
      font-weight: normal;
    }
  }

  .rightSide {
    margin-right: 30px;
  }

  ul li {
    display: inline-block;
    margin-left: 30px;

    .language { color: #BBC9E0; font-size: 13px; }
    .logIn { color: #FF7272; font-size: 15px; }
    .downloadApp {
      font-size: 14px;
      font-weight: bold;
      padding: 10px 20px;
      border-radius: 5px;
      background-color: #FF5859;
      color: #E5EBEF;
    }

    a { 
      text-decoration: none; 
    }
  }
}
</style>