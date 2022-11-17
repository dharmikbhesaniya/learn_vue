<template lang="">
    <div>
        <!-- two way binding useing v-model -->
        <h1>two way binding</h1>
        <input type="text" name="" id="" v-model="count" />
        <h2>{{ count }}</h2>
    </div>
</template>
<script>
export default {
    name: "Twowaybinding",
    data() {
        return {
            count: 0,
        };
    },
};
</script>
<style scoped>
h1 {
    background-color: black;
}
</style>
