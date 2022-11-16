<template lang="">
    <div>
        <h2>{{ data.name }} &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {{ data.email }}</h2>
        <button v-on:click="getname(data.name)">show name</button>
    </div>
</template>
<script>
export default {
    name: "Printdata",
    props: {
        data: "object",
        getname: "function",
    },
};
</script>
<style lang=""></style>
