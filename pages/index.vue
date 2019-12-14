<template>
  <div>
    <!-- Banner -->
    <div class="w-full bg-gray-900 py-2">
      <div class="container mx-auto">
        <div class="md:flex items-center">
          <div class="md:w-1/2 order-2">
            <img src="https://via.placeholder.com/500?text=Banner+Home+Page" alt="" class="w-full object-contain rounded overflow-hidden" style="height:500px;">
          </div>
          <div class="md:w-1/2 text-gray-200 order-1 px-4 py-4">
            <h1 class="text-xl text-gray-400">YALE SCHOOL OF ARTS</h1>
            <h2 class="mb-4 text-4xl font-serif text-yellow-400 font-bold leading-none">Registration for 2019 open!</h2>
            <p class="mb-5">2019 Yale School of Art Admission Open House will be held Thursday, November 14th, Noon-4pm, Doors at 11:30am</p>
            <nuxt-link to="" class="py-2 px-4 rounded-full border-2 border-gray-200 text-gray-200 hover:bg-gray-200 hover:text-gray-900 inline-block">Register Now</nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div class="container mx-auto px-4 py-10">
      <div class="bg-yellow-400 inline-block my-10">
        <h3 class="text-5xl font-serif tracking-tight text-gray-800 font-bold -mt-12 md:-ml-5">
          YALE ARTS NEWS
        </h3>
      </div>
      <div class=" md:flex md:items-center bg-white  overflow-hidden">
        <div class="md:w-1/4">
          <a href="#">
            <img alt="Mickalene Thomas, 2019" src="https://via.placeholder.com/500?text=Events+images" class=" w-full h-full object-cover" >
          </a>
        </div>
        <div class="md:w-3/4 md:pl-8 px-4 py-8">
          <div class="text-sm text-gray-600">NOVEMBER 11, 2019</div>
          <a href="#" class="text-3xl tracking-tight text-gray-800 font-bold hover:underline block mb-2">
            2020 Presidential Visiting Fellow in Fine Arts: Mickalene Thomeas
          </a>
          <p>The Yale School of Art announces the appointment of Mickalene Thomas as the 2020 Presidential Visiting Fellow in Fine Arts. </p>
        </div>
      </div>
      <div class="md:flex -mx-4">
        <div class="md:w-1/3  bg-white mx-4 overflow-hidden mt-6">
          <a href="#" class="block">
            <img class="w-full h-48 object-cover" alt="Read more about the 2019 Hayden Distinguished Fellows." src="https://via.placeholder.com/300?text=Events+images">
          </a>
          <div class="px-4 py-8">
            <div class="text-sm text-gray-600">
              OCTOBER 15, 2019
            </div>
            <a href="#" class="text-2xl tracking-tight leading-tight text-gray-800 font-bold hover:underline ">
              Celebrating 150 Years of The Yale School Of Art
            </a>
          </div>
        </div>
        <div class="md:w-1/3 bg-white mx-4 overflow-hidden mt-6">
          <a href="#" class="block">
            <img class="w-full h-48 object-cover" alt="Read more about the 2019 Hayden Distinguished Fellows." src="https://via.placeholder.com/300?text=Events+images">
          </a>
          <div class="px-4 py-8">
            <div class="text-sm text-gray-600">
              SEPTEMBER 16, 2019
            </div>
            <a href="#" class="text-2xl tracking-tight leading-tight text-gray-800 font-bold hover:underline">
              Announcing The Autumn 2019 Hayden Distinguished Fellows and Visiting Artist
            </a>
          </div>
        </div>
        <div class="md:w-1/3 bg-white mx-4 overflow-hidden mt-6">
          <a href="#" class="block">
            <img class="w-full h-48 object-cover" alt="Read more about the 2019 Hayden Distinguished Fellows." src="https://via.placeholder.com/300?text=Events+images">
          </a>
          <div class="px-4 py-8">
            <div class="text-sm text-gray-600">
              SEPTEMBER 16, 2019
            </div>
            <a href="#" class="text-2xl tracking-tight leading-tight text-gray-800 font-bold hover:underline">
            Meleko Mokgosi Appointed Associate Professor in Painting/Printmaking
            </a>
          </div>
        </div>
      </div>
      </div>

    </div>
  </div>
</template>

<script>

export default {
  components: {
  },
  head(){
    return {
        title: 'Yale School Of the Arts',
    }
  },
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

</style>
