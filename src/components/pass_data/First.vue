<template lang="">
    <div>
        <h1>chailde</h1>
        <h1>{{ name }}</h1>
        <h1>{{ user.name }}</h1>
        <button v-on:click="getdata()">call function</button>
    </div>
</template>
<script>
export default {
    name: "First",
    props: {
        name: "string",
        user: "object",
        getdata: "function",
    },
};
</script>
<style lang=""></style>
