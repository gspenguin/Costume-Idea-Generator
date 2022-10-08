<template>

  <h1>Costume Idea Generator</h1>
  Not sure what your halloween Costume should be?

  <Form />
</template>

<script>
import Form from './components/Form'
export default {
  name: "App",
  components: {
    Form
  },
};
</script>

<style>
  body  {
    background-color: orange;
    margin: 0;
    padding: 0;
    min-height: 90vh
  }
  #app {
    background-color: tan;
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    padding-top: 60px;
    width: 75%;
    margin: 0 auto;
  }
</style>
