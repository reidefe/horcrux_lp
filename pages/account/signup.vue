<template>
    <div class="flex flex-col md:flex-row bg-gradient-to-br from-purple-500 to-pink-500 min-h-screen">
      <div class="md:w-1/2 p-8">
        <h2 class="text-2xl font-bold text-white mb-6">Welcome back</h2>
        <p class="text-white mb-4">Please Enter your Account details</p>
        <div class="mb-4">
          <input type="email" v-model="email" placeholder="Email" class="w-full px-4 py-2 rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-600">
        </div>
        <div class="mb-4">
          <input type="password" v-model="password" placeholder="Password" class="w-full px-4 py-2 rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-600">
        </div>
        <div class="flex items-center mb-6">
          <input type="checkbox" id="keepLoggedIn" v-model="keepLoggedIn" class="mr-2">
          <label for="keepLoggedIn" class="text-white">Keep me logged in</label>
          <button class="ml-auto text-white underline focus:outline-none">Forgot Password</button>
        </div>
        <button @click="login" class="bg-white text-purple-500 font-bold py-2 px-6 rounded-lg focus:outline-none hover:bg-purple-100">
          Sign in
        </button>
        <div class="flex justify-center mt-6">
          <a href="#" class="mx-2"><img src="google-icon.png" alt="Google" class="w-8 h-8"></a>
          <a href="#" class="mx-2"><img src="facebook-icon.png" alt="Facebook" class="w-8 h-8"></a>
          <a href="#" class="mx-2"><img src="twitter-icon.png" alt="Twitter" class="w-8 h-8"></a>
        </div>
      </div>
      <div class="md:w-1/2 p-8 bg-black bg-opacity-50 text-white">
        <h2 class="text-2xl font-bold mb-6">What's our Jobseekers Said.</h2>
        <blockquote class="mb-6">
          "Search and find your dream job is now easier than ever.<br>
          Just browse a job and apply if you need to."
        </blockquote>
        <div class="flex items-center">
          <img src="avatar.png" alt="Avatar" class="w-12 h-12 rounded-full mr-4">
          <div>
            <p class="font-bold">Mas Parjono</p>
            <p>UI Designer at Google</p>
          </div>
        </div>
        <div class="mt-8">
          <p class="mb-4">Get your right job and right place apply now</p>
          <p class="mb-4">Be among the first founders to experience the easiest way to start run a business.</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        email: '',
        password: '',
        keepLoggedIn: false,
      };
    },
    methods: {
      login() {
        // Handle login logic here
        console.log('Login clicked');
      },
    },
  };
  </script>