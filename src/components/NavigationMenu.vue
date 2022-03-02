<template>
  <nav class="bg-red-600 p-4 flex justify-between">
    <h1 class="text-white text-2xl">{{ title }}</h1>
    <ToggleMenu />
  </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import ToggleMenu from "@/components/ToggleMenu.vue";

export default defineComponent({
  name: "NavigationMenu",
  components: {
    ToggleMenu,
  },
  data() {
    return {
      title: "D&D Tools",
    };
  },
  methods: {
    doSomething() {
      console.log("Lets do this!");
    },
  },
});
</script>
