<template>
<div>
    <ul>
        <li v-for="ninja in ninjas" :key="ninja"> {{ninja}} </li>  
    </ul>
   </div>
</template>

<script>

export default {
  name: 'app',
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

<style>

</style>
