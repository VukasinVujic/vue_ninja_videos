<template>

<div>

<h1>Computed Propertis</h1>
<button v-on:click="a++">Add to a</button>
<button v-on:click="b++">Add to b</button>

<button v-on:click="c++">Add to c</button>

<p> C = {{c}} </p>

<p> A = {{a}} </p>
<p> B = {{b}} </p>

<!-- for methods  -->
<!-- <p> age + A = {{addToA()}} </p> 
<p> age + B = {{addToB()}} </p> -->

<!-- for computed  -->
<p> age + A = {{addToA}} </p> 
<p> age + B = {{addToB}} </p>



</div>
</template>

<script>
export default {
  data(){
    return{
      name: 'VUkasin',
      age:20,
      a:0,
      b:0,
      c:0
    };
  },
  
  methods: {
      
      // addToA(){
      //   console.log('aaaaaaaaaaaa');
      //   return this.a + this.age;
      // },
      // addToB(){
      //   console.log('BBBBBBBB');
      //   return this.b + this.age;
      // }
  },
      computed: {
        addToA(){
        console.log('aaaaaaaaaaaa');
        return this.a + this.age;
      },
      addToB(){
        console.log('BBBBBBBB');
        return this.b + this.age;
      }
        
      }
           
  

};
</script>

    

<style>

#canvas {
  width: 600px;
  padding: 200px 20px;
  text-align: center;
  border: 1px solid #333;
}

</style>
