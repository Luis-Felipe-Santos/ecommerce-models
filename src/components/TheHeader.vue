<template>
  <header>
    <div class="pitchbar">
      <div class="pitchbar-items">
        <img src="../assets/left-arrow.svg" alt="left-arrow" />
        <p>
          <span>Frete grátis</span> a partir de <span>R$ 199,99</span> para todo
          o Brasil!
        </p>
        <img src="../assets/right-arrow.svg" alt="right-arrow" />
      </div>
    </div>
    <div class="header-meio">
      <nav class="navegacao">
        <div class="logo-icon">
          <router-link to="/" class="logo">
            <img src="../assets/logo-icon.svg" alt="Models" />
          </router-link>
        </div>
        <div class="busca">
          <img src="../assets/busca.svg" alt="buscar" />
          <input type="text" id="txtPesquisar" placeholder="Pesquisar por..." />
        </div>
        <div class="acoes">
          <div class="icone-carrinho">
            <img src="../assets/carrinho.svg" alt="" />
          </div>
          <div class="usuario">
            <div class="icone-usuario">
              <img src="../assets/user.svg" alt="" />
            </div>
          </div>
          <div class="login-usuario">
            <p class="bem-vindo">Seja bem vindo(a)!</p>
            <a class="entre">Entre</a>
          </div>
        </div>
      </nav>
    </div>
    <div class="menu-wrapper">
      <div class="menu">
        <div class="menu-nav">
          <ul>
            <div class="item1">
              <li>
                <img src="../assets/menu.svg" alt="menu" />
                Todas as categorias
              </li>
            </div>
            <div class="item2">
              <li>Smartphones</li>
            </div>
            <div class="item3">
              <li>Notebooks</li>
            </div>
            <div class="item4">
              <li>Consoles</li>
            </div>
            <div class="item5">
              <li>Headphones</li>
            </div>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "TheHeader",
};
</script>
<style scoped>
.pitchbar {
  width: 100%;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 8px 75px 8px 75px;
  background-color: blue;
}
.pitchbar-items {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  max-width: 1248px;
  height: 24px;
  padding: 0px 16px 0px 16px;
  background-color: aliceblue;
  gap: 12px;
}

span {
  font-weight: bold;
}
.header-meio {
  width: 100vw;
  height: 112px;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0 75px 0 75px;
  background-color: pink;
}
.navegacao {
  width: 100%;
  max-width: 1248px;
  height: 112px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0px 16px;
  background-color: #667085;
}

.busca {
  display: flex;
  width: 500px;
  padding: 10px 14px;
  gap: 8px;
  border: 1px solid #d7dae0;
  border-radius: 8px;
}
.busca input {
  width: 444px;
  border: none;
  color: #667085;
  size: 16px;
  line-height: 24px;
}
.acoes {
  width: 281px;
  height: 48px;
  display: flex;
  gap: 12px;
}
.icone-carrinho {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 48px;
  height: 48px;
  cursor: pointer;
}
.icone-usuario {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 48px;
  height: 48px;
  cursor: pointer;
}
.login-usuario {
  width: 130px;
  height: 40px;
}
.bem-vindo {
  width: 130px;
  height: 20px;
  color: #1861dd;
  size: 14px;
  line-height: 20px;
}
.entre {
  width: 36px;
  height: 20px;
  color: #b3b9c6;
  size: 14px;
  line-height: 20px;
  text-decoration: underline solid;
  cursor: pointer;
}
.menu-wrapper {
  width: 100%;
  height: 42px;
  padding: 0 96px;
  border-top: 1px solid #edeef1;
  border-bottom: 1px solid #edeef1;
  background-color: #1861dd;
}

.menu {
  width: 1248px;
  height: 42px;
  background-color: red;
}

.menu-nav {
  display: flex;
  width: 100%;
  max-width: 624px;
  height: 42px;
}

.menu ul {
  display: flex;
  align-items: center;
  padding: 12px 20px;
  gap: 8px;
}
.menu ul li {
  display: flex;
  gap: 8px;
  cursor: pointer;
}
.item1 {
  display: flex;
  align-items: center;
  width: 200px;
  height: 42px;
  padding: 12px 20px;
  gap: 8px;
}
.item2 {
  display: flex;
  align-items: center;
  width: 116px;
  height: 42px;
  padding: 12px 20px;
}
.item3 {
  display: flex;
  align-items: center;
  width: 103px;
  height: 42px;
  padding: 12px 20px;
}
.item4 {
  display: flex;
  align-items: center;
  width: 93px;
  height: 42px;
  padding: 12px 20px;
}
.item5 {
  display: flex;
  align-items: center;
  width: 112px;
  height: 42px;
  padding: 12px 20px;
}
</style>
