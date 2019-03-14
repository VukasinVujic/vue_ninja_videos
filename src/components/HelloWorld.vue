<template>

<div>
  <h1>Dynamic CSS</h1>
  <h2>Example 1</h2>
  <!-- <div v-on:click="available = !available" v-bind:class="{available: available}">
  <span>trrrruuuuu</span>
  </div> -->
  <h3>Example 2</h3>
  <button v-on:click="nearby =!nearby">Toggle nearby</button>
  <button v-on:click="available =!available">Toggle available</button>

<div v-bind:class="compClasses">
<span>aaaa</span>

</div>



</div>
</template>

<script>
export default {
  data(){
    return{
      available: false,
      nearby: false
     
    };
  },
  
  methods: {
      
     
  },
   computed: {
    compClasses(){
      return {
        available: this.available,
        nearby: this.nearby
      }
    }    
  }
           
  

};
</script>

    

<style>

span{
    background: red;
    display: inline-block;
    padding: 10px;
    color: #fff;
    margin: 10px 0;
}

.available span{
    background: green;
}

.nearby span:after{
    content: "nearby";
    margin-left: 10px;
}

</style>
