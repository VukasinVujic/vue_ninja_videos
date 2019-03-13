<template>

<div>

<h1> Events  </h1>
<button v-on:click.once="add(1)">Add a year</button>
<!-- <button v-on:click="age++">Add a year</button>  -->
<!-- ako je funkcija kraca moze odmah i ovde da se ispise -->
<button v-on:click="substract(1)">Substract a year</button>
<button v-on:dblclick="add(10)">Add 10 years</button>
<button v-on:dblclick="substract(10)">Substract 10 years</button>


 <p>My age is : {{age}} </p>

<div id="canvas" v-on:mousemove="updateXY"> {{x}} , {{y}} </div>
<a v-on:click.prevent="click" href="https://academy.vivifyideas.com/">video 6</a>


</div>
</template>

<script>
export default {
  data(){
    return{
      age:25,
      x:0,
      y:0
    };
  },
  
  methods: {
      add(inc){
        this.age +=inc;
      },
      substract(inc){
        this.age -=inc;
      },
      updateXY(event){
        this.x = event.offsetX;
        this.y = event.offsetY;
      },
      click(){
        alert('You clicked me');
      }     
  }

}
</script>

    

<style>

#canvas {
  width: 600px;
  padding: 200px 20px;
  text-align: center;
  border: 1px solid #333;
}

</style>
