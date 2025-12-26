<template>
  <appHeader></appHeader>
  <div 
  class="p-4 rounded" 
  :class="{ 'bg-red-500 text-white': isError, 'bg-gray-100 text-black': !isError }"
>
  <h1 class="text-5xl font-bold mb-4">Welcome to My Vue.js App</h1>
  <p class="mb-2">This is a simple Vue.js application demonstrating component usage and data binding.</p>
  <button 
    class="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600"
    @click="isError = !isError"
  >
    Toggle Error State
  </button>
</div>
<div style="text-align:center;  font-size:20px; gap: 50px; margin-top:30px;">
  <p >My name is :{{name}}</p>
<br>
<p>My age is :{{age}}</p>
<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minima sunt ut labore omnis illum tenetur veritatis natus consequatur sit! Impedit, esse sapiente odit placeat illo illum, suscipit nulla tempora aspernatur, hic deleniti consectetur voluptate. Esse nobis non deserunt iusto alias aliquid quis porro nemo. Eum aliquam numquam rem dolor provident ex, est, necessitatibus excepturi ipsa labore magni officia! Totam, expedita. Illo consequatur asperiores molestiae! Molestiae, sit? Quidem expedita possimus debitis itaque magni ducimus pariatur adipisci? Magni mollitia eligendi id esse eum adipisci dolores maxime sit architecto sunt error ipsam voluptatum voluptatem explicabo provident, sequi earum tempore, nisi, commodi autem cum.</p>
</div>
<appFooter></appFooter>
</template>

<script>
  import appHeader from './components/header_footer/header.vue';
  import appFooter from './components/header_footer/footer.vue';

export default {
  data(){
    return {
      name : "My name is sajjad Hossain JIM",
      age : 24
    }
  }
   ,
    components: {
      appHeader,
      appFooter
    }
};
</script>

<style>

</style>