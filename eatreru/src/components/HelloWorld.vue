<template>
  <div class="app">
    <h1>EAT Club &copy;RERU</h1>
<input type="text" v-model="font">
<Mycomponent :font="font" /><br>
Num1 :<input v-model.number="num1"><br>
Num2 :<input v-model.number="num2">
<!-- <p>{{result}}</p> -->
<p>Nmuber 1 :{{num1}}</p>
<p>Number 2 :{{num2}}</p>
<p>{{num1+num2}}</p>
<!-- <p>{{result}}</p> -->
</div>
</template>

<script>
  import Mycomponent from './Mycomponent'
  export default {
    name :'',
    num1: '',
    num2: '',
    // result: num1+num2,
    comments : {
      Mycomponent
    },
    data () {
      return {
        font:"Hello EAT"
      }
    }
  }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
