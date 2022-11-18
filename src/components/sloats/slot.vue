<template lang="">
    <div>
        <slot>this is a slot</slot>
        <h4>{{ name }}</h4>
    </div>
</template>
<script>
export default {
    name: "slot",
    props: {
        name: "string",
    },
};
</script>
<style lang=""></style>
