<template lang="">
    <div>
        <div>{{ tag }}</div>
        <!-- nothing write here because this is error throw -->
        <h1>hello</h1>
        <div v-html="tag"></div>
    </div>
</template>
<script>
export default {
    name: "Htmabinding",
    data() {
        return {
            tag: "<h1> hello </h1>",
        };
    },
};
</script>
<style lang=""></style>
