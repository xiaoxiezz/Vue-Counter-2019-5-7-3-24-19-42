<template>
  <div class="counter">
    <p >{{number}}</p>
    <button v-on:click="add">+</button>
    <button v-on:click="reduce">-</button>
  </div>
</template>

<script>
export default {
        name: 'Counter',    
        data(){
            return {
                number: 0
            }
        },
 methods: {
     add: function(){
         this.number ++;
     },
     reduce: function(){
         this.number --;
     }
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
