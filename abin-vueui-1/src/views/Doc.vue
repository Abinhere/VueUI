<template>
    <Topnav/>
    <div class="content">
        <aside v-if="activeVisible">
            <h2>组件列表</h2>
            <ol>
                <li>
                    <router-link to="/doc/switch">Switch 组件</router-link>
                </li>
                <li>
                    <router-link to="/doc/button">Button 组件</router-link>
                </li>
                <li>
                    <router-link to="/doc/tabs">Tabs 组件</router-link>
                </li>
            </ol>
        </aside>
        <main>
            <router-view></router-view>
        </main>
    </div>
</template>

<script lang="ts">
import Topnav from '../components/Topnav.vue'
import {inject,Ref} from 'vue'
export default {
    components:{Topnav},
    setup() {
        const activeVisible = inject<Ref<boolean>>('activeVisible')
        return {activeVisible}
    }
}
</script>

<style lang="scss" scoped>
.content{
    display: flex;
    height: 500px;
    > aside{
        flex: 1;
        margin-right: 10px;
        background: lightblue;
        width: 150px;
        padding: 16px;
        > h2{
            margin-bottom: 4px;
        }
        > ol{
            > li{
                padding: 4px 0;
            }
        }
        @media (max-width: 500px){
            position: fixed;
            top: 0;
            left: 0;
            padding-top: 70px;
        }
    }
    > main{
        background:white;
        flex: 8;
        margin-left: auto;
        overflow-y: auto;
    }
}
</style>