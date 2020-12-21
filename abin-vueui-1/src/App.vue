<template>
  <router-view/>
</template>

<script lang="ts">
import { provide, ref } from 'vue'
export default {
  name: 'App',
  setup() {
    const width = document.documentElement.clientWidth;
    const activeVisible = ref(width <= 300 ? false:true);
    provide ('activeVisible',activeVisible)
  }
}
</script>
