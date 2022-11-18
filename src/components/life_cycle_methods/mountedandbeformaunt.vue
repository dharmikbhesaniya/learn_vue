<template lang="">
    <div>
        <h1>this is a life cycle methods of mounted and beformount</h1>
        <p>{{ name }}</p>
    </div>
</template>
<script>
export default {
    name: "mountedandbeformaunt",
    data() {
        console.log("created");
        return {
            name: "test",
        };
    },
    beforeMount() {
        console.log("beforemount", this.$el);
    },
    mounted() {
        console.log("bmounted", this.$el);
    },
};
</script>
<style lang=""></style>
