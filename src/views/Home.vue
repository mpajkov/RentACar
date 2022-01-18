<template>
  <div id="app">
    <div class="flex justify-evenly items-center img sss"><img src="@/assets/pocetna_edit.jpg" alt="Pocetna"></div>

    </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>

.nav-link{
  color:white !important;
}

.sss{
  top: 120px;
}

</style>