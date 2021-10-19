<template>
  <div class="flex flex-col justify-center items-center h-screen">
    <img alt="Vue logo" src="../assets/logo.png">
    <landing msg="Welcome to FabStars App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Landing from '@/components/Landing.vue';

export default {
  name: 'Home',
  components: {
    Landing,
  },
};
</script>
