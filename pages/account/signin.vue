<template>
    <div class="min-h-screen bg-gradient-to-br from-purple-900 to-indigo-900 flex items-center justify-center">
      <div class="bg-white bg-opacity-10 rounded-lg shadow-lg p-8 max-w-md w-full">
        <h2 class="text-2xl font-bold text-white mb-6">Sign In</h2>
        <p class="text-gray-300 mb-8">Keep it all together and you'll be fine</p>
        <div class="mb-4">
          <input type="email" v-model="email" placeholder="Email or Phone" class="w-full bg-white bg-opacity-20 text-white px-4 py-2 rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-600 placeholder-gray-400">
        </div>
        <div class="mb-4">
          <input type="password" v-model="password" placeholder="Password" class="w-full bg-white bg-opacity-20 text-white px-4 py-2 rounded-lg focus:outline-none focus:ring-2 focus:ring-purple-600 placeholder-gray-400">
        </div>
        <button @click="forgotPassword" class="text-purple-400 hover:underline focus:outline-none mb-8">
          Forgot Password
        </button>
        <button @click="signIn" class="bg-purple-600 text-white font-bold py-2 px-6 rounded-lg w-full focus:outline-none hover:bg-purple-700 mb-4">
          Sign In
        </button>
        <div class="text-center">
          <p class="text-gray-400 mb-4">or</p>
          <button @click="signInWithApple" class="bg-black text-white font-bold py-2 px-6 rounded-lg focus:outline-none hover:bg-gray-800">
            Sign in with Apple
          </button>
        </div>
        <p class="text-gray-400 text-center mt-8">New to Atomz? <a href="/account/signup/" class="text-purple-400 hover:underline focus:outline-none">Join Now</a></p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        email: '',
        password: '',
      };
    },
    methods: {
      signIn() {
        // Handle sign in logic here
        console.log('Sign In clicked');
      },
      forgotPassword() {
        // Handle forgot password logic here
        console.log('Forgot Password clicked');
      },
      signInWithApple() {
        // Handle sign in with Apple logic here
        console.log('Sign in with Apple clicked');
      },
    },
  };
  </script>