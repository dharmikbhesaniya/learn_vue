<template lang="">
    <div>
        <!-- two way binding useing v-model -->
        <input type="text" name="" id="" v-model="email" />
        <br />
        <br />
        <input type="text" name="" id="" v-model="pass" />
        <br /><br />
        <h1>{{ email }}</h1>
        <h1>{{ pass }}</h1>
        <br /><br />

        <input type="checkbox" name="" value="java" id="java" v-model="tech" />
        <label for="java">java</label>

        &nbsp;&nbsp;&nbsp;&nbsp;
        <input
            type="checkbox"
            name=""
            value="javascript"
            id="javascript"
            v-model="tech"
        />
        <label for="javascript">javascript</label>
        <h1>{{ tech }}</h1>

        <br /><br /><br />
        <input
            type="radio"
            name="fa"
            value="devloper"
            id="devloper"
            v-model="info"
        />
        <label for="devloper">devloper</label>
        &nbsp;&nbsp;&nbsp;&nbsp;
        <input
            type="radio"
            name="fa"
            value="programar"
            id="programar"
            enable
            v-model="info"
        />
        <label for="programar">programar</label>
        <h1>{{ info }}</h1>
        <br /><br />
        <button type="button" v-on:click="getdata()">get value</button>
        <br /><br />
    </div>
</template>

<script>
export default {
    name: "Valuegetfrominput",
    data() {
        return {
            form: {
                email: null,
                pass: null,
                tech: [],
                info: "",
            },
        };
    },
    methods: {
        getdata() {
            console.log(`Email: ${this.email}`);
            console.log(`pass: ${this.pass}`);
            console.log(`tech: ${this.tech}`);
            console.log(`info: ${this.info}`);
        },
    },
};
</script>

<style lang=""></style>
