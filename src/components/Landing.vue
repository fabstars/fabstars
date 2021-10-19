<template>
  <div class="p-5">
    <h1 class="text-3xl">{{ msg }}</h1>
    <div class="flex flex-col pt-3">
      <div class="flex flex-row">
        <h1 class="text-xl font-bold">FabStars.com/</h1>
        <div class="pl-1">
          <input type="text" class="border border-gray-400 rounded mb-4">
        </div>
      </div>
      <div class="pt-3">
        <button class="bg-blue-500 hover:bg-blue-700
        text-white font-bold py-2 px-4 rounded" type="submit" >Start my page!</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Landing',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
