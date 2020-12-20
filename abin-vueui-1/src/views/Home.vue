<template>
    <div>
        <Topnav/>
        <div class="banner">
            <h1>轮子UI</h1>
            <h2>UI框架</h2>
            <p class="actions">
                <a>GitHub</a>                
                <a>开始</a>
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
    > h1,h2{
        font-weight:bold;
    }
}
</style>