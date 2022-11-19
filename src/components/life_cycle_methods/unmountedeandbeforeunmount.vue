<template lang="">
    <div>
        <h1>unmountede and beforeunmount</h1>
        <button v-on:click="show = !show">hide and show</button>
        <bindwithunmountVue v-if="show" />
    </div>
</template>
<script>
import bindwithunmountVue from "./bindwithunmount.vue";
export default {
    name: "unmountedeandbeforeunmount",
    data() {
        return {
            show: true,
        };
    },
    components: {
        bindwithunmountVue,
    },
    
};
</script>
<style lang=""></style>
