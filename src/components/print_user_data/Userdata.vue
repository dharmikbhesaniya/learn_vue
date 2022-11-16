<template lang="">
    <div>
        <!-- useing loop many time use component with pass data and primt data -->
        <ul>
            <li v-for="item in user">
                <Printdata :data="item" :getname="getname" />
            </li>
        </ul>
    </div>
</template>
<script>
import Printdata from "./Printdata.vue";

export default {
    name: "Userdata",
    components: {
        Printdata,
    },
    methods: {
        getname(name) {
            alert(name);
        },
    },
    data() {
        return {
            user: [
                { name: "peter", email: "abc@xyz.com" },
                { name: "peter1", email: "abc1@xyz.com" },
                { name: "peter2", email: "abc2@xyz.com" },
                { name: "peter3", email: "abc3@xyz.com" },
                { name: "peter4", email: "abc4@xyz.com" },
            ],
        };
    },
};
</script>
<style lang=""></style>
