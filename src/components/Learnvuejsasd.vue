<template lang="">
  <div>
    <h3>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dicta rem
      eveniet in asperiores doloremque itaque aperiam minima excepturi dolorum
      quo quisquam assumenda id distinctio eligendi sed, vitae fuga et quibusdam
      iusto nostrum laborum possimus! Earum optio nulla, quae vel fugit
      perferendis nam perspiciatis? Esse tempore voluptates commodi non,
      repellendus sapiente quas laboriosam distinctio aliquid et quod quibusdam
      mollitia, recusandae debitis, eos officia quisquam porro dolorem aliquam
      dolorum sed cum id enim obcaecati? Soluta iure porro officia temporibus
      tenetur vitae, corporis aperiam in sunt. Mollitia nihil repellendus
      voluptate voluptatum expedita exercitationem, doloremque delectus! Sint
      minima esse mollitia minus possimus quod suscipit!
    </h3>
    <h1>{{ mobile }}</h1>
    <h1>{{ mobile == 222 }}</h1>
    <h1>{{ (mobile = 222) }}</h1>
    <h1>{{ mobile == 222 }}</h1>
    <h3>{{ getname("dharmik") }}</h3>
    <h1>{{ get() }}</h1>
  </div>
</template>

<script>
export default {
  name: "Learnvuejsasd",
  data() {
    return {
      mobile: 111,
    };
  },
  methods: {
    getname(name) {
      return `my name is ${name}`;
    },
    get() {
      return this.mobile;
    },
  },
};
</script>

<style scoped>
h3 {
  color: aqua;
}
</style>
