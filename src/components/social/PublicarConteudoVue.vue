<template>
  <div class="row">
    <GridVue class="input-field" tamanho="12">
      <textarea v-model="conteudo" class="materialize-textarea"></textarea>
      <label>Oque está acontecendo?</label>
    </GridVue>
    <p>
      <GridVue
        v-if="conteudo"
        class="btn waves-effect waves-light"
        tamanho="2 offset-s10"
      >
        Publicar
      </GridVue>
    </p>
  </div>
</template>

<script>
import GridVue from "@/components/layouts/GridVue.vue";

export default {
  name: "PublicarConteudoVue",
  components: {
    GridVue
  },
  data() {
    return {
      conteudo: ""
    };
  }
};
</script>

<style></style>
