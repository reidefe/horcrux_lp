<template>
    <div class="flex justify-center">
      <div
        class="rounded-lg shadow-lg bg-white max-w-sm mx-auto overflow-hidden md:max-w-md lg:max-w-lg"
      >
        <img
          class="w-full h-48 object-cover"
          src="https://picsum.photos/800/600"
          alt="Profile Cover"
        />
        <div class="p-4 md:p-6 lg:p-8">
          <div class="flex items-center mb-4">
            <img
              class="w-16 h-16 rounded-full object-cover mr-4"
              src="https://picsum.photos/200"
              alt="Profile Picture"
            />
            <div>
              <h2 class="text-xl font-semibold">John Doe</h2>
              <p class="text-gray-600">Web Developer</p>
            </div>
          </div>
          <p class="text-gray-700 mb-4">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed
            consequat, tortor eget faucibus tincidunt, eros pede varius ipsum, quis
            condimentum mauris turpis vitae metus.
          </p>
          <div class="flex justify-center space-x-4">
            <a
              href="#"
              class="text-gray-600 hover:text-gray-800 transition-colors duration-300"
            >
              <i class="fab fa-facebook fa-lg"></i>
            </a>
            <a
              href="#"
              class="text-gray-600 hover:text-gray-800 transition-colors duration-300"
            >
              <i class="fab fa-twitter fa-lg"></i>
            </a>
            <a
              href="#"
              class="text-gray-600 hover:text-gray-800 transition-colors duration-300"
            >
              <i class="fab fa-instagram fa-lg"></i>
            </a>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ProfileVue',
  }
  </script>