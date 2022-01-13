<template>
  <div class="social-networks">
    <social-link name="Github" to="https://www.github.com/" icon="github.svg" />
    <social-link
      name="Twitter"
      to="https://www.twitter.com/"
      icon="twitter.svg"
    />
    <social-link
      name="Facebook"
      to="https://www.facebook.com/"
      icon="facebook.svg"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { SocialLink } from "@/components/atoms"

export default defineComponent({
  components: {
    SocialLink,
  },
});
</script>

<style lang="scss" scoped>
.social-networks {
  display: grid;
  grid-gap: 1rem;
}
</style>
