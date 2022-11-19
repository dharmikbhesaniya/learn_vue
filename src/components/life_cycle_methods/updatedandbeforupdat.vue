<template lang="">
    <div>
        <h1 ref="coun">{{ count }}</h1>
        <button v-on:click="count = count + 1">update count</button>
    </div>
</template>
<script>
export default {
    name: "updatedandbeforupdat",
    data() {
        return {
            count: 0,
        };
    },
    beforeUpdate() {
        // this is a ui throw use and call
        console.log("this is a beforeupdate", this.count);
        console.log("this is a beforeupdate", this.$refs["coun"].textContent);
    },
    updated() {
        console.log("this is a update", this.count);
        console.log("this is a update", this.$refs["coun"].textContent);
    },
};
</script>
<style lang=""></style>
