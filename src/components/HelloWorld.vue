<template>

<div>

  <h1> {{greet("afternoon")}}  </h1>
 <p>Name: {{name}}</p>
  <p>Job: {{job}} </p>


</div>
</template>

<script>
export default {
  data(){
    return{
      name:"Shaun",
      job:"arbeit",

    };
  },
  
  methods: {
    greet(time){
      this.name
     return "Good " + time + ' ' + this.name;
    }
  }

}
</script>

    

<style>

</style>
