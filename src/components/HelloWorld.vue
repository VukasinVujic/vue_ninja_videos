<template>

<div>

<h1>Keyboard events </h1>
<label>Name:</label>
<input type="text" v-on:keyup.enter="logName">
<label>Age</label>
<input type="text" v-on:keyup.enter.alt="logAge">



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
      },
      logName(){
        console.log('you enter your name');
      },
      logAge(){
        console.log('you enter you age');
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
