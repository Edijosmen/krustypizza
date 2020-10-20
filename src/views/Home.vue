<template>
  <div class="home">
    <Homeuser/>
  </div>
  
</template>

<script>
// @ is an alias to /src
import Homeuser from '@/components/Homeuser.vue'
export default {
  name: 'Home',
  components: {
    Homeuser
  }
}
</script>
