<template lang="">
    <div>
        <h1 ref="user">bind with unmount</h1>
    </div>
</template>
<script>
export default {
    name: "bindwithunmount",
    // this life cycle is call to hide a component
    beforeUnmount() {
        console.log("beforeUnmount", this.$refs["user"]);
    },
    unmounted() {
        console.log("Unmounted", this.$refs["user"]);
    },
};
</script>
<style lang=""></style>
