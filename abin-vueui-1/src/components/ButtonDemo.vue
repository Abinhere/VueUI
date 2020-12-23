<template>
    <div>
        Button 的文档
    </div>
    <h1>示例1</h1>
    <div>
        <Button>哇嘎</Button>
        <Button theme="button">
            哇嘎
        </Button>
        <Button theme="link">
            哇嘎
        </Button>
        <Button theme="text">
            哇嘎
        </Button>
    </div>
    <h1>示例2</h1>
    <div>
        <Button size="big" theme="button">
            哇嘎
        </Button>
        <Button theme="button">哇嘎</Button>
        <Button size="small" theme="button">
            哇嘎
        </Button>
    </div>
    <div>
        <Button size="big" theme="link">
            哇嘎
        </Button>
        <Button theme="link">哇嘎</Button>
        <Button size="small" theme="link">
            哇嘎
        </Button>
    </div>
    <div>
        <Button size="big" theme="text">
            哇嘎
        </Button>
        <Button theme="text">哇嘎</Button>
        <Button size="small" theme="text">
            哇嘎
        </Button>
    </div>
    <div>
        <Button size="big" level="main" theme="button">
            哇嘎
        </Button>
        <Button theme="button">哇嘎</Button>
        <Button size="small" level="danger" theme="button">
            哇嘎
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