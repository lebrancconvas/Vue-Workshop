<template>
  <div class="hello">
    <h1>{{ nameweb }}</h1>
    <h1>{{ msg }}</h1>
    <h2>Join your party and fight for league.</h2>
    <button class="butt" v-on:click="say('I choose you')">{{ dec }}</button>
    <p>{{ pika }}</p>
  </div>

</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      /* เขียนตัวแปรลงช่องนี */
      nameweb:'Pokevue',
      msg: 'Welcome to my Pokemon Website',
      dec: 'Hello Trainer',
      pika: 100
    }
  },
  methods: {
    say: function (message) {
      alert(message)
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
.butt{
  background-color: #f72d2d; /* Green */
  border: none;
  color: white;
  width : 100px;
  height: 100px;
  -moz-border-radius: 50px;
  -webkit-border-radius: 50px;
  border-radius: 50px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 14px;
}
</style>
