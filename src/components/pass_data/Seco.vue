<template lang="">
    <div>
        <First name="dharmik" :user="user" :getdata="getdata"/>
        <p>perant</p>
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
        };
    },
    methods: {
        getdata() {
            console.log("hello");
        },
    },
};
</script>
<style lang=""></style>
