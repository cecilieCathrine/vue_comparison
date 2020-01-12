<template>
  <div class="travel">
    <h2>{{msg}}</h2>
    <button @click="pickCountry()">Get me somewhere</button>
    <span v-if="randomCountry">You should go to <strong>{{ randomCountry }}</strong> </span>
  </div>
</template>

<script>
import { countries } from "../jsonData/countries";
export default {
  name: 'WhereToGo',
  props: {
    msg: String
  },
  data() {
    return {
      randomCountry: ""
    }
  },
  methods: {
    pickCountry () {
      this.randomCountry = countries[Math.floor(Math.random() * countries.length)].name;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  background-color: white;
  border: 2px solid #008CBA;
  color: black;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  font-size: 16px;
  margin: 4px 2px;
  -webkit-transition-duration: 0.4s; /* Safari */
  transition-duration: 0.4s;
  cursor: pointer;
  margin: auto;
  display: block;
  margin-bottom: 2em;
}
button:hover {
  background-color: #008CBA;
  color: white;
}
</style>
