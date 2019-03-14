<template>

<div>

<h1>Keyboard events </h1>
<label>Name:</label>
<input type="text" v-model="name">
<span> {{name}} </span>
<label>Age</label>
<input type="text" v-model="age" >
<span> {{age}} </span>



</div>
</template>

<script>
export default {
  data(){
    return{
      name: 'VUkasin',
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
        
      },
      logAge(){
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
