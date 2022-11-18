<template lang="">
<div>
    <!-- two way binding useing v-model with velidetion -->
    <input type="text" name="" id="" v-model="form.email" />
    <br />
    <br />
    <input type="text" name="" id="" v-model="form.pass" />
    <br /><br />
    <h1>{{ form.email }}</h1>
    <h1>{{ form.pass }}</h1>
    <br /><br />

    <input type="checkbox" name="" value="java" id="java" v-model="form.tech" />
    <label for="java">java</label>

    &nbsp;&nbsp;&nbsp;&nbsp;
    <input type="checkbox" name="" value="javascript" id="javascript" v-model="form.tech" />
    <label for="javascript">javascript</label>
    <h1>{{ form.tech }}</h1>

    <br /><br /><br />
    <input type="radio" name="fa" value="devloper" id="devloper" v-model="form.info" />
    <label for="devloper">devloper</label>
    &nbsp;&nbsp;&nbsp;&nbsp;
    <input type="radio" name="fa" value="programar" id="programar" enable v-model="form.info" />
    <label for="programar">programar</label>
    <h1>{{ form.info }}</h1>
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
                email: "",
                pass: "",
                tech: [],
                info: "",
            },
            error: [],
        };
    },
    methods: {
        getdata() {
            this.error = [];
            for (let i in this.form) {
                if (this.form[i] === "" || this.form[i].length === 0) {
                    this.error.push(i);
                }
            }
            if (this.error.length < 1) {
                console.log(`Email: ${this.form.email}`);
                console.log(`pass: ${this.form.pass}`);
                console.log(`tech: ${this.form.tech}`);
                console.log(`info: ${this.form.info}`);
                alert("sucsess");
            } else {
                console.log(this.error);
            }
        },
    },
};
</script>

<style lang=""></style>
