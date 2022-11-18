<template lang="">
    <div>
        <slotVue>
            <h1>this is a print useing slot</h1>
        </slotVue>
        <slotVue name="dharmik"></slotVue>

        <multislotVue>
            <template v-slot:header>
                <h1>this is a first multi slot</h1>
            </template>
            <template v-slot:body>
                <h1>this is a second multi slot</h1>
            </template>
            <template v-slot:footer>
                <h1>this is a threed multi slot</h1>
            </template>
        </multislotVue>
    </div>
</template>

<script>
import slotVue from "./slot.vue";
import multislotVue from "./multislot.vue";
export default {
    name: "main.vue",
    components: {
        slotVue,
        multislotVue,
    },
};
</script>

<style lang=""></style>
