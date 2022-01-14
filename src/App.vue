<template>
  <div class="component">
    <Header />
    <h4>StartDayJs - {{ startDateDayjs }}</h4>
    <h4>EndDayJs - {{ endDateDayjs }}</h4>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Header } from "@/components/organisms";

import dayjs from "dayjs";

export default defineComponent({
  components: {
    Header,
  },
  setup() {
    return {
      startDateDayjs: dayjs().subtract(3, "months").format("YYYY-MM-DD"),
      endDateDayjs: dayjs().add(1, "days").format("YYYY-MM-DD"),
    };
  },
});
</script>

<style lang="scss" scoped>
.component {
  margin: 1rem;
}
</style>
