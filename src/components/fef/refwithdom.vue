<template lang="">
    <div>
        <!-- use ref with dom and cantrol a dom -->
        <input type="text" name="a" ref="in" id="" />
        <input type="text" name="" id="" />
        <button v-on:click="dom">submit</button>
        <h1>this is your last value</h1>
        <h3>{{ val }}</h3>
    </div>
</template>
<script>
export default {
    name: "refwithdom",
    data() {
        return {
            val: "",
        };
    },
    methods: {
        dom() {
            this.$refs.in.focus();
            this.val = this.$refs.in.value;
        },
    },
};
</script>
<style lang=""></style>
