<template>
  <header id="header" class="bg-gray-700">
    <nav class="container mx-auto flex justify-start items-center py-5 px-4">
    <!-- App Name -->
      <router-link class="text-white font-bold uppercase text-2xl mr-4"
      :to="{name: 'Home'}">
      Fab Stars
      </router-link>
      <div class="flex flex-grow items-center">
        <!-- Primary Navigation -->
        <ul class="flex flex-row mt-1">
          <!-- Navigation Links -->
          <li v-if="true">
            <a class="px-2 text-white" href="#">
              Login / Register
            </a>
          </li>
          <template v-else>
            <li>
              <router-link class="px-2 text-white" to="/">Manage</router-link>
            </li>
            <li>
              <a class="px-2 text-white" href="#">Logout</a>
            </li>
          </template>
          <li>
              <router-link class="px-2 text-white" :to="{name: 'About'}">About</router-link>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'header',
};
</script>

<style>
#header a.router-link-exact-active {
  color: #42b983;
}
</style>
