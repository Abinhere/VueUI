<template>
  <router-view/>
</template>

<script lang="ts">
import { provide, ref } from 'vue'
import { router } from './router'
export default {
  name: 'App',
  setup() {
    const width = document.documentElement.clientWidth;
    const activeVisible = ref(width <= 300 ? false:true);
    provide ('activeVisible',activeVisible);
    router.afterEach(()=>{
      if(width<=800){
        activeVisible.value = false;
      }
    })
  }
}
</script>
