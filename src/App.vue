<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import { BeakerIcon } from "@heroicons/vue/solid";
import { ref } from "vue";

const count = ref(0);

const addCount = () => {
  count.value++;
};
</script>

<template>
  <h1 class="text-3xl font-bold underline text-red-400">Hello world!</h1>
  <BeakerIcon class="h-5 w-5 text-blue-500" @click="addCount" />
  <div>
    {{ count }}
  </div>

  <RouterView />
</template>
