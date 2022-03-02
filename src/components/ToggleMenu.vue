<template>
  <div class="relative">
    <MenuAlt3Icon
      @click="showMenu = !showMenu"
      class="h-8 w-8 text-white lg:hidden active:bg-blue cursor-pointer"
    />
    <div
      v-if="showMenu"
      class="lg:hidden absolute h-fit w-max p-2 bg-red-600 border-2 border-red-400 -bottom-20 -left-20 flex flex-col space-y-1 rounded shadow-lg"
    >
      <a class="text-white cursor-pointer">Dice Generator</a>
      <a class="text-white cursor-pointer">Spells</a>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "@vue/runtime-core";
import { MenuAlt3Icon } from "@heroicons/vue/outline";

export default defineComponent({
  name: "ToggleMenu",
  components: {
    MenuAlt3Icon,
  },
  data() {
    return {
      showMenu: false,
    };
  },
});
</script>
