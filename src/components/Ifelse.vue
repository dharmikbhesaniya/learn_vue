<template lang="">
    <div>
        <h1 v-if="sho">hello</h1>
        <h1 v-else>hello</h1>
    </div>
</template>
<script>
export default {
    name: "Ifelse",
    data() {
        return {
            sho: true,
        };
    },
};
</script>
<style lang=""></style>
