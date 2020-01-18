<template>
  <div class="hello">
    <form action>
      <input type="text" placeholder="text" v-model="text">
      <input type="submit" value="decided" @click="submitClick">
    </form>
  </div>
</template>

<script>
// import Axios from "axios";
export default {
  name: "HelloWorld",
  data() {
    return {
      text: null
    };
  },
  methods: {
    submitClick() {
      alert(this.text)
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
