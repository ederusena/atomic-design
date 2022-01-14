<template>
  <div class="services">
    <Service
      title="Frontend"
      description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius odit beatae nam recusandae autem ea delectus ullam, doloribus voluptates nostrum praesentium tempora unde facere error, explicabo, velit voluptatem nobis voluptate?"
    />

    <Service
      title="Backend"
      description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius odit beatae nam recusandae autem ea delectus ullam, doloribus voluptates nostrum praesentium tempora"
    />
    <Service
      title="Computer Science"
      description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius odit beatae nam recusandae autem ea delectus ullam, doloribus voluptates nostrum praesentium tempora"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Service } from "@/components/molecules";

export default defineComponent({
  components: {
    Service,
  },
});
</script>

<style scoped lang="scss">
.services {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 5rem;
}
</style>
