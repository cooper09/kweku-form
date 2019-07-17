<template>
  <div class="hello">
    <h1>Main Form</h1>
    <input label='name' name='name' type="text" size="%50" /><br/>
    <input label='address' name='address' type="text" size="%50" /><br/>
    <input label='serialNo' name='serialNo' type="text" size="%50" /><br/>
    <br/>
    <button v-on:click="onClick">Submit</button>
  </div>
</template>

<script>
export default {
  name: 'Form',
  data() {
     return {
         form: {
             name: null,
             age:null
         }
     } 
  },//end data
  methods: {
      onClick: function() {
          alert("Let's Go!")
          console.log("Form submitted: ", this.form )
      }
    }//end methods
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
