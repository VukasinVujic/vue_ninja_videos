<template>

<div>

<h1>Data binding</h1>
  <!-- <h1> {{greet("afternoon")}}  </h1> -->
 <a v-bind:href="website"> link za sa sajt</a>
 <!-- skracenica dole od ovog gore -->
 <!--  <a :href="website"> link za sa sajt</a> -->
<input type="text" v-bind:value="job">

  <p v-html="websiteTag"></p>

</div>
</template>

<script>
export default {
  data(){
    return{
      name:"Shaun",
      job:"arbeit",
      website: "https://www.google.rs/",
      websiteTag: '<a href="https://www.google.rs/"> aaaa </a> '
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
