<template>
  <nav class="nav-bar">
    <nav-item text="Serviços" to="/services" />
    <nav-item text="Sobre mim" to="/about" />
    <nav-item text="Cases" to="/cases" />
    <nav-item text="Contato" to="/contact" />
  </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { NavItem } from "@/components/atoms";

export default defineComponent({
  components: {
    NavItem,
  },
  props: {
    text: {
      type: String,
      required: true,
    },
    to: {
      type: String,
      required: true,
    },
  },
});
</script>

<style scoped>
.nav-bar {
  width: max-content;
  display: grid;
  grid-auto-flow: column;
  grid-gap: 2.5rem;
}
</style>
