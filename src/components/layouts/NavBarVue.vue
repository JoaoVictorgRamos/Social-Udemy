<template>
  <nav :class="cor || 'blue'">
    <div class="nav-wrapper container">
      <router-link :to="url || '#/'" class="brand-logo">{{
        logo || "Logo"
      }}</router-link>
      <ul id="nav-mobile" class="right hide-on-med-and-down">
        <slot></slot>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  props: ["logo", "url", "cor"],
  data() {
    return {};
  }
};
</script>

<style></style>
