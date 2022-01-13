<template>
  <div class="component">
    <logo />
    <nav-bar />
    <search-form />
    <social-networks />
    <service title="Front End" description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt eius hic dolores ratione rem ipsam quisquam asperiores, architecto quasi perspiciatis quos porro esse? Vero quasi dignissimos consequatur id saepe sit?" />
    <service title="Back End" description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt eius hic dolores ratione rem ipsam quisquam asperiores, architecto quasi perspiciatis quos porro esse? Vero quasi dignissimos consequatur id saepe sit?" />
    <service title="Web Development" description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt eius hic dolores ratione rem ipsam quisquam asperiores, architecto quasi perspiciatis quos porro esse? Vero quasi dignissimos consequatur id saepe sit?" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import {
  NavBar,
  SearchForm,
  SocialNetworks,
  Service,
} from "@/components/molecules";
import { Logo } from "@/components/atoms";

export default defineComponent({
  components: {
    Logo,
    NavBar,
    Service,
    SearchForm,
    SocialNetworks,
  },
});
</script>

<style lang="scss" scoped>
.component {
  width: 300px;
}
</style>
