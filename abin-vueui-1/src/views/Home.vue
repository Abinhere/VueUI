<template>
    <div>
        <Topnav/>
        <div class="banner">
            <h1>轮子UI</h1>
            <h2>UI框架</h2>
            <p class="actions">
                <a href="https://github.com/Abinhere/VueUI">GitHub</a>                
                <router-link to="/doc">开始</router-link>
            </p>
        </div>
    </div>
</template>
<script lang="ts">
import Topnav from '../components/Topnav.vue'
export default {
    components:{Topnav}
}
</script>

<style lang="scss" scoped>
.banner{
    text-align: center;
    background:plum;
    border-radius: 0 0 50% 50%;
    > .actions{
        padding: 8px 0;
        a{
            margin: 0 8px;
            background: #fff;
            display: inline-block;
            $h:28px;
            height: $h;
            line-height: $h;
            border-radius: $h/2;
            padding: 0 8px;
        }
    }
}
</style>