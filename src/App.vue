<template>
<div>
  <h1> {{title}} </h1>
  <ninjas>  </ninjas>

   </div>
</template>

<script>
import Ninjas from './components/Ninjas.vue'

export default {
  components: {
    Ninjas
  },

  name: 'app',
  data(){
    return {
      title: 'Ninja app'
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
  color:purple 
}

</style>
