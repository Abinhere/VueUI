<template>
    <div>
        Button 的文档
    </div>
    <h1>示例1</h1>
    <div>
        <Button @click="onClick" @focus="onClick" @mouseover="onClick">
            哇嘎雷共
        </Button>
    </div>
</template>
<script lang="ts">
import Button from '../lib/Button.vue'
export default {
    components:{Button},
    setup() {
        const onClick = ()=>{
            console.log('h1');
        }
        return {onClick};
    }
}
</script>