<template lang="">
    <div>
        <h1>this is a life cycle methods of created and beforcrete</h1>
        <p>{{ name }}</p>
    </div>
</template>

<script>
export default {
    name: "createdandbeforcreate",
    data() {
        console.log("created");
        return {
            name: "test",
        };
    },
    beforeCreate() {
        this.name = "befor";
        alert("this is beforcrate");
    },
    created() {
        this.name = "after";
        alert("this is aftercrate");
    },
};
</script>

<style lang=""></style>
