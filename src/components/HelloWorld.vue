<template>
  <div class="hello">
    <h3>{{ msg }}</h3>
    <Form />

  </div>
</template>

<script>

import Form from '@/components/Form.vue';
import axios from 'axios';

export default {
  name: 'HelloWorld',
  components: { 
    Form
  },
  props: {
    msg: String
  }
}
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
