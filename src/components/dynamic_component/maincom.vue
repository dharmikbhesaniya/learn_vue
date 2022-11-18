<template lang="">
    <div>
        <button @click="tab = 'firstVue'">first</button>
        <button @click="tab = 'secondVue'">second</button>
        <button @click="tab = 'therrdVue'">threed</button>

        <component :is="tab" />
    </div>
</template>
<script>
import firstVue from "./first.vue";
import secondVue from "./second.vue";
import therrdVue from "./therrd.vue";
export default {
    name: "maincom",
    data() {
        return {
            tab: "",
        };
    },
    components: {
        firstVue,
        secondVue,
        therrdVue,
    },
};
</script>
<style lang=""></style>
