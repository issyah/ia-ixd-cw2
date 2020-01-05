<template>
  <div>
    <div class="flex h-screen items-center justify-center">
      <div class="md:w-1/2">
        <form class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4">
          <h1 class="text-2xl font-semibold">Login</h1>
          <div class="mb-4">
            <label class="block text-gray-700 text-sm font-bold mb-2" for="username">
              Username
            </label>
            <input class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="username" type="text" placeholder="Username">
          </div>
          <div class="mb-6">
            <label class="block text-gray-700 text-sm font-bold mb-2" for="password">
              Password
            </label>
            <input class="shadow appearance-none  rounded w-full py-2 px-3 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline" id="password" type="password" placeholder="******************">
          </div>
          <div class="flex items-center justify-between">
            <button class="bg-yellow-500 hover:shadow-md rounded-full py-2 px-4 rounded focus:outline-none focus:shadow-outline" type="button">
              Sign In
            </button>
            <a class="inline-block align-baseline font-bold text-sm text-blue-500 hover:text-blue-800" href="#">
              Forgot Password?
            </a>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    head(){
      return{
        head: 'Login'
      }
    }
  }
</script>
