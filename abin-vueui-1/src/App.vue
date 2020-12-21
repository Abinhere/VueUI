<template>
  <router-view/>
</template>

<script lang="ts">
import { provide, ref } from 'vue'
export default {
  name: 'App',
  setup() {
    const activeVisible = ref(false)
    provide ('xxx',activeVisible)
  }
}
</script>
