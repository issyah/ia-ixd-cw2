<template>
  <div>
    <!-- banner -->
    <div class="w-full bg-gray-900 py-10 relative">
      <div class="container mx-auto pb-20 flex items-center relative" style="height:500px;">
        <div class="self-center">
          <div class="text-center">
            <div class="bg-gray-700 inline-block my-10">
              <h1 class="text-center font-serif text-6xl font-bold text-yellow-400 -mt-12 md:-ml-5">Graduate Programmes</h1>
            </div>
          </div>
          <div class="text-center px-4">
            <h4 class="text-gray-400 text-2xl">The Yale School of Art is a graduate school that confers Master of Fine Arts Degrees in Graphic Design, Painting/Printmaking, Photography, and Sculpture</h4>
          </div>
        </div>
      </div>
    </div>
    .
    <div class="container mx-auto md:-mt-56 mb-10 relative">
      <!-- Main information -->
      <div class="md:flex md:flex-wrap md:-mx-4">
        <div class="md:w-1/2 overflow-hidden mt-8 px-4" v-for="item in programmes">
          <div class="bg-gray-900 text-gray-200 shadow-xl h-full">
            <nuxt-link :to="item.url">
              <img :src="item.img" class="w-full h-56 object-cover">
            </nuxt-link>
            <div class="px-10 py-10">
              <nuxt-link :to="item.url">
                <h2 class="font-bold text-4xl text-yellow-400 font-serif inline-block hover:underline">{{item.title}}</h2>
              </nuxt-link>
              <h4 class="text-lg leading-relaxed mt-5">{{item.content}}</h4>
              <div class="text-right mt-6">
                <nuxt-link :to="item.url" class="btn-programmes">
                  Learn more
                </nuxt-link>
              </div>
          </div>
          </div>
        </div>
        <!-- <div class="md:w-1/2 bg-gray-700 text-gray-200 shadow-xl overflow-hidden mt-6 mx-4">
          <img src="https://via.placeholder.com/500?text=Painting+Printmaking" class="w-full h-56 object-cover">
          <div class="px-10 py-10">
            <h2 class="font-bold text-4xl text-yellow-400 font-serif">Painting & Printmaking</h2>
            <h4 class="text-lg leading-relaxed mt-5">Instruction in the program is rooted in the investigation of painting as a unique genre with its own complex syntax and history. Within this setting, the program encourages diversity of practice and interpretation, innovation, and experimentation.</h4>
            <div class="text-right mt-10">
              <nuxt-link to="#" class="btn-programmes">
                Learn more
              </nuxt-link>
            </div>
          </div>
        </div> -->
      </div>
    </div>
  </div>
</template>

<script>

export default {
  data:()=>({
    programmes:[
      {
        title:'Graphic Design',
        img:'https://via.placeholder.com/600?text=Graphic+Design',
        content:'The graphic design program focuses on the development of a cohesive, investigative body of work, also known as the student’s thesis. At Yale, the graphic design thesis is conceived as a loose framework within which each student’s visual method is deployed across many diverse projects during the two-year course of study.',
        url:'/graduate-programmes/graphic-design'
      },
      {
        title:'Painting & Printmaking',
        img: 'https://via.placeholder.com/600?text=Painting+Printmaking',
        content:'Instruction in the program is rooted in the investigation of painting as a unique genre with its own complex syntax and history. Within this setting, the program encourages diversity of practice and interpretation, innovation, and experimentation.',
        url:'#'
      },
      {
        title:'Photography',
        img: 'https://via.placeholder.com/600?text=Photography',
        content:'Photography is a two-year program of study admitting ten students a year. Darkroom, studio, and computer facilities are provided. Students receive technical instruction in black-and-white and color photography as well as nonsilver processes and digital image production.',
        url:'#'
      },
      {
        title:'Sculpture',
        img: 'https://via.placeholder.com/600?text=Sculpture',
        content:'The sculpture program offers students the opportunity to develop their work in a supportive environment consisting of critical feedback in a broad array of diverse voices. The field of sculpture includes a varied collection of working methods and outcomes—one set of tools is not privileged over another—creating a healthy and experimental program that mirrors the issues facing artists outside of the institution',
        url:'#'
      }
    ]
  }),
  head(){
    return {
      title: 'Graduates Programmes - Yale',
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

.btn-programmes{
  @apply py-2 px-4 rounded-full border-2 border-gray-200 text-gray-200 inline-block
}
.btn-programmes:hover{
  @apply bg-gray-200 text-gray-900
}
</style>
