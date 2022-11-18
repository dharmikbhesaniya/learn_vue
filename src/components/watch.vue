<template lang="">
    <div>
        <h1>{{ count }}</h1>
        <button v-on:click="cou">+</button>
        <button v-on:click="coun">-</button>
    </div>
</template>
<script>
export default {
    name: "watch",
    data() {
        return {
            count: 0,
        };
    },
    watch: {
        // function name is same also data name
        count() {
            if (this.count > 5) {
                this.count = 0;
            } else if (this.count < 0) {
                this.count = 5;
            }
        },
    },
    methods: {
        cou() {
            this.count = this.count + 1;
        },
        coun() {
            this.count = this.count - 1;
        },
    },
};
</script>
<style lang=""></style>
