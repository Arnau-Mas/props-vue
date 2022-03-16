<template>
  <div class="hello">
    <h1>{{title}}</h1>
    <slot></slot>
    <p>{{content}}</p>
    <Button :buttonText="buttonText"></Button>
  </div>
</template>

<script>
import Button from './Button.vue'
export default {
  components: { Button },
  props:{
    title:{
      type:String
    },
    content:{
      type:String
    },
    buttonText:{
      type:String
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.hello{
  width: 20rem;
  border: 1px #42b983 solid;
  box-shadow: 5px 5px #42b983;
  margin-bottom: 2rem;
  padding: 1rem;
}
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
