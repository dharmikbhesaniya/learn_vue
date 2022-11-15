<template lang="">
    <div>
        <ul>
            <li v-for="i in num">
                {{ i }}
            </li>
        </ul>
        <ul>
            <li v-for="i in boj">{{ i.name }} {{ i.email }}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "Forloop",
    data() {
        return {
            num: [1, 2, 3, 4, 5],
            boj: [
                {
                    name: "dharmik",
                    email: "ds@gmail.coms",
                },
                {
                    name: "meet",
                    email: "meet@gmail.com",
                },
            ],
        };
    },
};
</script>

<style lang=""></style>
