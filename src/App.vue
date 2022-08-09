<template>
  <base-container class="sm:p-8">
    <default-box v-for="item in list" :key="item.id" :highlight="item.promo">
      {{ item.title }}
    </default-box>
  </base-container>
</template>

<script>
import BaseContainer from "./shared/BaseContainer.vue";
import DefaultBox from "./shared/DefaultBox.vue";
export default {
  components: { BaseContainer, DefaultBox },
  setup() {
    const list = [
      { id: 1, title: "Tailwind Css" },
      { id: 2, title: "Tailwind Css", promo: true },
      { id: 3, title: "Tailwind Css" },
      { id: 4, title: "Tailwind Css" },
      { id: 5, title: "Tailwind Css" },
      { id: 6, title: "Tailwind Css" },
      { id: 7, title: "Tailwind Css", promo: true },
      { id: 8, title: "Tailwind Css" },
      { id: 9, title: "Tailwind Css" },
    ];
    return { list };
  },
};
</script>
