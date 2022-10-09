<template>
  <span id="app">
    <header>
      <NavBarVue logo="Social" cor="green darken-3" url="/">
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/login">Login</router-link></li>
        <li><router-link to="/cadastro">Cadastro</router-link></li>
      </NavBarVue>
    </header>
    <main>
      <div class="container">
        <div class="row">
          <GridVue tamanho="8">
            <CardMenuVue>
              <slot name="menuEsquerdo"></slot>
            </CardMenuVue>
          </GridVue>
          <GridVue tamanho="4">
            <slot name="principal"></slot>
          </GridVue>
        </div>
      </div>
    </main>
    <FooterVue
      logo="Social"
      cor="green darken-3"
      descricao="Teste de descicao"
      ano="2022"
    >
      <li><a class="grey-text text-lighten-3" href="#!">Link 1</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>
    </FooterVue>
  </span>
</template>

<script>
import NavBarVue from "@/components/layouts/NavBarVue.vue";
import FooterVue from "@/components/layouts/FooterVue.vue";
import GridVue from "@/components/layouts/GridVue.vue";
import CardMenuVue from "@/components/layouts/CardMenuVue.vue";
export default {
  name: "LoginTemplate",
  components: {
    NavBarVue,
    FooterVue,
    GridVue,
    CardMenuVue
  }
};
</script>

<style></style>
