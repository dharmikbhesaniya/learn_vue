<template>
    <div>
        <!-- this is bind in index.html -->
        <Teleport to="#teleport">
            <teleportcomponentVue />
        </Teleport>

        <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
        <!-- <learnvuejsasd /> -->
        <!-- <twowaybinding /> -->
        <!-- <Valuegetfrominput /> -->
        <!-- <Ifelse /> -->
        <!-- <Forloop /> -->
        <!-- <seco /> -->
        <!-- <secos /> -->
        <!-- <userdata /> -->
        <!-- <Htmlbinding /> -->
        <!-- <classbinding /> -->
        <!-- <refwithdom /> -->
        <!-- <watch /> -->
        <!-- <mai /> -->
        <!-- <maincom /> -->
        <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    </div>
</template>

<script>
import teleportcomponentVue from "./components/teleportcomponent.vue";
import Forloop from "./components/Forloop.vue";
import HelloWorld from "./components/HelloWorld.vue";
import Ifelse from "./components/Ifelse.vue";
import Learnvuejsasd from "./components/Learnvuejsasd.vue";
import Twowaybinding from "./components/binding/Twowaybinding.vue";
import Valuegetfrominput from "./components/binding/Valuegetfrominput.vue";
import Seco from "./components/pass_data/Seco.vue";
import Secos from "./components/two_way_pass_data/Seco.vue";
import Userdata from "./components/print_user_data/Userdata.vue";
import Htmlbinding from "./components/binding/Htmlbinding.vue";
import classbinding from "./components/binding/classbinding.vue";
import refwithdom from "./components/fef/refwithdom.vue";
import watch from "./components/watch.vue";
import mai from "./components/sloats/main.vue";
import maincom from "./components/dynamic_component/maincom.vue";
export default {
    name: "App",
    components: {
        teleportcomponentVue,
        HelloWorld,
        Learnvuejsasd,
        Twowaybinding,
        Valuegetfrominput,
        Ifelse,
        Forloop,
        Seco,
        Secos,
        Userdata,
        Htmlbinding,
        classbinding,
        refwithdom,
        watch,
        mai,
        maincom,
    },
};
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
