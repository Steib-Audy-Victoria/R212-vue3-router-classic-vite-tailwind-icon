<template>
  <main class="bg-indigo-25">
    <div class="grid place-content-center">
      <div class="xl:hidden">
        <h2 class="text-4xl font-bold leading-10">Search properties to rent</h2>
        <div class="m-4 flex justify-between rounded-md border-2 border-indigo-100 bg-white p-2">
          <p class="text-base font-medium leading-6 text-gray-900">Search with Search Bar</p>
          <IconSearchBar></IconSearchBar>
        </div>
        <div class="m-4 flex justify-between rounded-md bg-white">
          <p class="flex items-center p-2 text-base font-medium leading-6 text-gray-500">Search location</p>
          <IconButtonSearch></IconButtonSearch>
        </div>
      </div>
      <div class="hidden xl:block">
        <div class="m-4 flex justify-between rounded-md bg-white">
          <div>
            <p class="flex items-center p-2 text-base font-medium leading-6 text-gray-500">Location</p>
            <p class="flex items-center p-2 text-lg font-bold leading-7 text-gray-900">New York, USA</p>
          </div>
          <div>
            <p class="flex items-center p-2 text-base font-medium leading-6 text-gray-500">Location</p>
            <p class="flex items-center p-2 text-lg font-bold leading-7 text-gray-900">New York, USA</p>
          </div>
          <div>
            <p class="flex items-center p-2 text-base font-medium leading-6 text-gray-500">Location</p>
            <p class="flex items-center p-2 text-lg font-bold leading-7 text-gray-900">New York, USA</p>
          </div>
          <div>
            <p class="flex items-center p-2 text-base font-medium leading-6 text-gray-500">Location</p>
            <p class="flex items-center p-2 text-lg font-bold leading-7 text-gray-900">New York, USA</p>
          </div>
          <IconButtonSearch2></IconButtonSearch2>
        </div>
      </div>
    </div>
    <div class="grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(400px,1fr))] justify-items-center p-2">
      <card nom="Beverly Springfield" :prix="5000" :favori="true" image="/public/pexels-binyamin-mellish-106399.jpg" :bath="2"></card>
      <card nom="Beverly Springfield" :prix="5000" favori image="/public/pexels-binyamin-mellish-106399.jpg" :bath="2"></card>
      <card nom="Beverly Springfield" :prix="5000" image="/public/pexels-binyamin-mellish-106399.jpg" :bath="2"></card>
      <card nom="Beverly Springfield" :prix="5000" image="/public/pexels-binyamin-mellish-106399.jpg" :bath="2"></card>
      <card nom="Beverly Springfield" :prix="5000" image="/public/pexels-binyamin-mellish-106399.jpg" :bath="2"></card>
      <card nom="Beverly Springfield" :prix="5000" image="/public/pexels-binyamin-mellish-106399.jpg" :bath="2"></card>
    </div>
  </main>
</template>

<script>
import IconSearchBar from "../components/icons/IconSearchBar.vue";
import IconButtonSearch from "../components/icons/IconButtonSearch.vue";
import IconButtonSearch2 from "../components/icons/IconButtonSearch2.vue";

import card from "../components/card.vue";

export default {
  components: { IconSearchBar, IconButtonSearch, IconButtonSearch2, card },
};
</script>