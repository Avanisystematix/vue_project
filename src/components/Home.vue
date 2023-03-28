<template>
  <div class="main">
    <h1>hello</h1> 
    <!-- to pass data -->
    <!-- <h1>{{ data }}</h1> -->

    <!-- events -->
    <!-- <button v-on:click="hello">Submit</button>  -->

    <!-- conditions -->
    <!-- <h1 v-if="show">conditional rendring if</h1>
    <h1 v-else>conditional rendring else</h1>
    <button v-on:click="display">Toggle element</button> -->

    <!-- loops -->
    <table>
      <tr>
        <th>Id</th>
        <th>Name</th>
        <th>Email</th>
      </tr>
      <tr v-for="user in users" :key="user.id">
        <td>{{ user.id }}</td>
        <td>{{ user.name }}</td>
        <td>{{ user.email }}</td>
      </tr>
    </table>
    
  </div>
</template>

<script>
export default {
name: "Home",

// to pass data
props:{
  data:String
},

// events
// methods:{
//   hello() {
//      console.log("hello");
//   },
//   hello(data){
//     alert(data)
//   }
// },

//loops
data(){
  return {
    users:[
      {id:2,name:"test2",email:"test2@test.com"},
      {id:3,name:"test3",email:"test3@test.com"},
      {id:4,name:"test4",email:"test4@test.com"},
    ]
  }
}

}
</script>

<style>

</style>