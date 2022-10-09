<template>
  <SiteTemplate>
    <span slot="menuEsquerdo">
      <div class="row valign-wrapper">
        <GridVue tamanho="4">
          <img
            src="http://archives.materializecss.com/0.100.2/images/yuna.jpg"
            alt=""
            class="circle responsive-img"
          />
          <!-- notice the "circle" class -->
        </GridVue>
        <GridVue tamanho="8">
          <span class="black-text">
            <h5>Maria Silva</h5>
            Add the "circle" class to it to make it appear circular.
          </span>
        </GridVue>
      </div>
    </span>
    <span slot="principal">
      <PublicarConteudoVue></PublicarConteudoVue>
      <CardConteudoVue
        perfil="//archives.materializecss.com/0.100.2/images/yuna.jpg"
        nome="Maria Silva"
        data="12/01/18 | 12;31"
      >
        <CardDetalheVue
          img="//archives.materializecss.com/0.100.2/images/sample-1.jpg"
          titulo=""
          txt="I am a very simple card. I am good at containing small bits of information. I am convenient because I require little markup to use effectively."
        ></CardDetalheVue>
      </CardConteudoVue>
    </span>
  </SiteTemplate>
</template>

<script>
import SiteTemplate from "@/templates/SiteTemplate";
import CardConteudoVue from "@/components/social/CardConteudoVue";
import CardDetalheVue from "@/components/social/CardDetalheVue";
import PublicarConteudoVue from "@/components/social/PublicarConteudoVue.vue";
import GridVue from "@/components/layouts/GridVue.vue";

export default {
  name: "Home",
  components: {
    SiteTemplate,
    CardConteudoVue,
    CardDetalheVue,
    PublicarConteudoVue,
    GridVue
  },
  data() {
    return {};
  }
};
</script>

<style scoped></style>
