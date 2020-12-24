<template>
    <div>
        Button 的文档
    </div>
    <h1>不同类型</h1>
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
    <h1>size</h1>
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
    <h1>禁用</h1>
    <div>
        <Button disabled>Hi</Button>
        <Button disabled theme="text">Hi</Button>
        <Button disabled theme="link">Hi</Button>
    </div>
    <h1>loading</h1>
    <div>
        <Button loading>加载中...</Button>
        <Button loading theme="text">加载中...</Button>
        <Button loading theme="link">加载中...</Button>
        <Button >加载完毕</Button>
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