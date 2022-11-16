<template lang="">
    <div>
        <h1 :class="apply">helloworld</h1>
        <button v-on:click="chan()">to chang bgcolor</button>&nbsp;&nbsp;&nbsp;
        <button v-on:click="chan1()">to chang textcolor</button
        >&nbsp;&nbsp;&nbsp;
        <button v-on:click="chan2()">to chang font size</button
        >&nbsp;&nbsp;&nbsp;
    </div>
</template>
<script>
export default {
    name: "classbinding",
    data() {
        return {
            bgcolo: true,
            colo: true,
            fon: true,
        };
    },
    computed: {
        apply() {
            return {
                h1: this.bgcolo,
                red: this.colo,
                fo: this.fon,
            };
        },
    },
    methods: {
        chan() {
            this.bgcolo = !this.bgcolo;
        },
        chan1() {
            this.colo = !this.colo;
        },
        chan2() {
            this.fon = !this.fon;
        },
    },
};
</script>
<style scoped>
.h1 {
    background-color: aqua;
    padding: 10px;
}
h1 {
    width: 200px;
}
.red {
    color: red;
}
.fo {
    font-size: 50px;
}
</style>
