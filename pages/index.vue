<template>
  <div>
    <!-- Banner -->
    <div class="w-full relative bg-gray-900 py-2 overflow-hidden ">
      <img class="object-cover absolute inset-0" alt="Background art" src="~/assets/images/banner.jpg"/>
      <div class="container mx-auto relative">
        <div class="md:flex items-center banner-content">
          <div class="md:w-1/2 order-2">
          </div>
          <div class="md:w-1/2 text-gray-200 order-1 px-8 py-8 bg-gray-900">
            <h1 class="text-xl text-gray-400">YALE SCHOOL OF ARTS</h1>
            <h2 class="mb-4 text-4xl font-serif text-yellow-400 font-bold leading-none">Registration for 2019 open!</h2>
            <p class="mb-5">2019 Yale School of Art Admission Open House will be held Thursday, November 14th, Noon-4pm, Doors at 11:30am</p>
            <nuxt-link to="" class="py-2 px-4 rounded-full border-2 border-yellow-400 text-yellow-400 hover:bg-yellow-400 hover:text-gray-900 inline-block">Register Now</nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div class="container mx-auto px-4 py-10">
      <div class="relative my-10 inline-block">
        <h3 class="text-5xl font-serif tracking-tight text-gray-800 font-bold relative z-10">
          YALE ARTS NEWS
        </h3>
        <div class="absolute bottom-0 h-5 w-full bg-yellow-400 mb-2"></div>
      </div>
      <div class=" md:flex md:items-center bg-white shadow overflow-hidden">
        <div class="md:w-1/4">
          <a href="#">
            <img alt="Mickalene Thomas, 2019" src="https://cdn.filestackcontent.com/aRMDlCPWRfOJWb6QOj8I" class=" w-full h-full object-cover" >
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
      <div class="md:flex -mx-4 ">
        <div class="md:w-1/3 shadow  bg-white mx-4 overflow-hidden mt-6">
          <a href="#" class="block">
            <img class="w-full h-48 object-contain bg-gray-800" alt="Read more about the 2019 Hayden Distinguished Fellows." src="https://cdn.filestackcontent.com/AFx79KQcETNaOd4KM3pL4z/http://art.yale.edu/image_columns/0016/1464/yale150_list12_09s_1920px_1_.gif">
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
        <div class="md:w-1/3 bg-white mx-4 overflow-hidden mt-6 shadow">
          <a href="#" class="block">
            <img class="w-full h-48 object-cover" alt="Read more about the 2019 Hayden Distinguished Fellows." src="https://cdn.filestackcontent.com/AFx79KQcETNaOd4KM3pL4z/resize=width:700/https://cdn.filepicker.io/api/file/2ytPTTV9T8iMY6u704JR/convert">
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
        <div class="md:w-1/3 bg-white mx-4 overflow-hidden mt-6 shadow">
          <a href="#" class="block">
            <img class="w-full h-48 object-cover" alt="Read more about the 2019 Hayden Distinguished Fellows." src="https://cdn.filestackcontent.com/resize=width:700/TSNLYI6aQM6Ok4RKt4oz">
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

.banner-content{
  height:550px;
}
@media (max-width:768px){
  .banner-content{
    height:auto;
  }
}

</style>
