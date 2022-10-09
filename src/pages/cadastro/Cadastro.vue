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
      <h2>Cadastro</h2>
      <input type="text" placeholder="Nome" />
      <input type="email" placeholder="E-mail" />
      <input type="password" placeholder="Senha" />
      <input type="password" placeholder="Confirme sua Senha" />
      <button class="btn">Enviar</button>
      <router-link class="btn orange" to="/login">
        Já tenho conta
      </router-link>
    </span>
  </LoginTemplate>
</template>

<script>
import LoginTemplate from "@/templates/LoginTemplate";
export default {
  name: "Cadastro",
  components: {
    LoginTemplate
  },
  data() {
    return {
      cadastro: true
    };
  }
};
</script>

<style></style>
