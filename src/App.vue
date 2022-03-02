<template>
  <NavigationMenu />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import NavigationMenu from "./components/NavigationMenu.vue";

export default defineComponent({
  name: "App",
  components: {
    NavigationMenu,
  },
});
</script>
