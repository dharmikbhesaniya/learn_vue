<template lang="">
    <div>
        <First name="dharmik" :user="user" :getdata="getdata" />
        <p>perant</p>
        <h1>{{ username }}</h1>
    </div>
</template>
<script>
import First from "./First.vue";

export default {
    name: "Seco",
    components: {
        First,
    },
    data() {
        return {
            user: { name: "peter", email: "peter@test.com" },
            username: "",
        };
    },
    methods: {
        getdata(name) {
            this.username = name;
        },
    },
};
</script>
<style lang=""></style>
