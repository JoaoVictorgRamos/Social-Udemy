<template>
  <LoginTemplate>
    <span slot="menuEsquerdo">
      <img
        src="https://blog.russelservicos.com.br/wp-content/uploads/2022/02/Conheca-as-vantagens-de-possuir-uma-rede-social-corporativa.png"
        alt="social"
        class="responsive-img"
      />
    </span>
    <span slot="principal">
      <h2>Login</h2>
      <input type="text" placeholder="email" />
      <input type="text" placeholder="senha" />
      <button class="btn">Entrar</button>
      <router-link class="btn orange" to="/cadastro">
        Cadastre-se
      </router-link>
    </span>
  </LoginTemplate>
</template>

<script>
import LoginTemplate from "@/templates/LoginTemplate";
export default {
  name: "Login",
  components: {
    LoginTemplate
  },
  data() {
    return {
      cadastro: false
    };
  }
};
</script>

<style></style>
