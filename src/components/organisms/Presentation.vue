<template>
  <div class="presentation">
    <SocialNetworks />
    <img
      src="@/assets/images/presentation.svg"
      alt="Aprensentação"
      class="presentationimg"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { SocialNetworks } from "@/components/molecules";

export default defineComponent({
  components: {
    SocialNetworks,
  },
  setup() {
    return {};
  },
});
</script>

<style lang="scss" scoped>
.presentation {
  position: relative;
  display: grid;
  justify-content: center;
  .presentationimg {
    width: 80%;
    justify-self: center;
  }
  .social-networks {
    position: absolute;
    left: 0;
    top: 50%;
    transform: translateY(-50%);
  }
}
</style>
