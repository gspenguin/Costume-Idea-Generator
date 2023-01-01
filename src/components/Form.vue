
<template>
  <div class="hello">
    <form>
      <div class="field">
        <label>Who is the costume for?</label>
        <select v-model="costumeFor">
          <option value="one_adult">One Adult</option>
          <option value="two_people">Two People</option>
          <option value="children">Children</option>
          <option value="group">Children</option>
        </select>
      </div>
    </form>
    <div>You selected {{ costumeFor }}</div>
    <button @click="getCostume">Get Costume Idea</button>
  </div>
</template>

<script>
import costumes from '../costumes.json'
export default {
  name: "Form",
  props: {
    msg: String,
  },
  methods: {
    getCostume(){

      alert(`Looking for costumes for ${this.costumeFor}`);
      alert(`How about ${costumes[this.costumesFor][0]}`)
    }
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
