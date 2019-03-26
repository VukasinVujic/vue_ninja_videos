<template>
<div>
  <h1>list of ninjas</h1>
    <ul>
        <li v-for="ninja in ninjas" :key="ninja"> {{ninja}} </li>  
    </ul>
   </div>
</template>

<script>

export default {
  data(){
    return {
      ninjas: ['Youshi', 'Mario', 'Ryu']
    }
  },
  methods : {
    greeting(){
      return 'heeey greeting text '
    }
  }
}
</script>

<style scoped>
h1 {
  color:green;
}
</style>
