<template>
    <div class="home">
      <!--<img alt="Vue logo" src="../assets/logo.png">-->
      <galaxy msg="Welcome to Your Universe's Webpage"/>
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
  import galaxy from '@/components/galaxy.vue'
  
  export default {
    name: 'HomeViewC',
    components: {
      galaxy
    }
  }
  </script>