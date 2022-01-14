<template>
  <header class="header">
    <logo />
    <nav-bar />
    <search-form />
  </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Logo } from "@/components/atoms";
import { NavBar, SearchForm } from "@/components/molecules";
export default defineComponent({
  components: {
    Logo,
    NavBar,
    SearchForm,
  },
  setup() {
    return {};
  },
});
</script>

<style scoped>
.header {
  width: 100%;
  display: grid;
  grid-template-columns: 160px repeat(2, auto);
  align-items: center;
  justify-content: space-between;
}
</style>
