<template>
  <header>
    <div class="flex justify-between p-5">
      <div class="flex">
        <icon-logo />
        <h1 class="text-xl font-bold leading-7 text-gray-900">Estratery</h1>
      </div>
      <IconMenu class="xl:hidden"></IconMenu>
      <nav class="hidden xl:block">
        <RouterLink to="/" class="text-blue-600 underline">Accueil</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<script>
import IconLogo from "./components/icons/IconLogo.vue";
import { FilmIcon } from "@heroicons/vue/outline";
import IconMenu from "./components/icons/IconMenu.vue";
export default {
  components: { IconLogo, FilmIcon, IconMenu },
};
</script>

<style>
</style>