<template>
    <div>
        <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
        <!-- <learnvuejsasd /> -->
        <!-- <twowaybinding /> -->
        <!-- <Valuegetfrominput /> -->
        <!-- <Ifelse /> -->
        <!-- <Forloop /> -->
        <seco />
        <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    </div>
</template>

<script>
import Forloop from "./components/Forloop.vue";
import HelloWorld from "./components/HelloWorld.vue";
import Ifelse from "./components/Ifelse.vue";
import Learnvuejsasd from "./components/Learnvuejsasd.vue";
import Twowaybinding from "./components/Twowaybinding.vue";
import Valuegetfrominput from "./components/Valuegetfrominput.vue";
import Seco from "./components/pass_data/Seco.vue";
export default {
    name: "App",
    components: {
        HelloWorld,
        Learnvuejsasd,
        Twowaybinding,
        Valuegetfrominput,
        Ifelse,
        Forloop,
        Seco,
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
