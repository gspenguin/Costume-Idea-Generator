<template>
  <div class="hello">
    <form>
      <div class="field">
        <label>Who is the costume for?</label>
        <select v-model="costumeFor">
          <option>One Adult</option>
          <option>Two People</option>
          <option>Children</option>
        </select>
      </div>
    </form>
    <div>You selected {{ costumeFor }}</div>
    <button>Get Costume Idea</button>
  </div>
</template>

<script>
export default {
  name: "Form",
  props: {
    msg: String,
  },
  data() {
    return {
      costumeFor: ''
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
