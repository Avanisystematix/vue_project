<template>
  <div>
    <h1>Templates</h1>
    <h2>{{ name }}</h2>
    <h2 v-once>{{ name }}</h2>
    <h3>{{ 10+10 }}</h3> 
    <h3>{{ a+b }}</h3> 
    <h3>{{ ok?"Yes":"No"}}</h3>
    <button v-on:click="updateText">Click me</button>
    <button v-bind:disabled="disableBtn">Click me</button>
  </div>
</template>

<script>
export default {
  name: "TemplateWithExample",
  data() 
  {
    return {
      name: 'Test',
      a:10,
      b:20,
      // if we have value for ok true then it will show yes else no
      ok:true,
      disableBtn:true
    }
  },
  methods:{
    updateText()
      {
        this.name="testit"
        // for button
        this.ok=!this.ok
      }
  }
};
</script>