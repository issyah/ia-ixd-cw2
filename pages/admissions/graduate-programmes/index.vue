<template>
  <div>
    <!-- banner -->
    <div class="w-full bg-gray-900 py-10 relative overflow-hidden graduate-programmes-banner">
      <div class="absolute inset-0 bg-gray-900 opacity-50">

      </div>
      <div class="container mx-auto pb-40 flex items-center relative" style="height:500px;">
        <div class="self-center">
          <div class="text-center">
            <div class="relative my-10 inline-block">
              <h1 class="text-6xl font-serif tracking-tight text-yellow-400 font-bold relative z-10">
                Graduate Programmes
              </h1>
              <div class="absolute bottom-0 h-5 w-full bg-gray-700 mb-2"></div>
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
            <div class="px-10 py-10 relative">
              <nuxt-link :to="item.url">
                <h2 class="font-bold text-4xl text-yellow-400 font-serif inline-block hover:underline">{{item.title}}</h2>
              </nuxt-link>
              <h4 class="text-lg leading-relaxed mt-5">{{item.content}}</h4>
              <div class="text-right mt-8">
                <nuxt-link :to="item.url" class="btn-cta">
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
<style>
.btn-cta{
  @apply py-2 px-4 rounded-full border-2 border-yellow-400 text-yellow-400 inline-block
}
.btn-cta:hover{
  @apply bg-yellow-400 text-gray-900
}

.graduate-programmes-banner{
  background:url('~assets/images/graduate-programmes.jpeg') 50% 50% no-repeat;
  background-size: cover;
}
</style>

<script>

export default {
  data:()=>({
    programmes:[
      {
        title:'Graphic Design',
        img:require('~/assets/images/graphic-design-2.jpeg'),
        content:'The graphic design program focuses on the development of a cohesive, investigative body of work, also known as the student’s thesis. At Yale, the graphic design thesis is conceived as a loose framework within which each student’s visual method is deployed across many diverse projects during the two-year course of study.',
        url:'/admissions/graduate-programmes/graphic-design'
      },
      {
        title:'Painting & Printmaking',
        img: require('~/assets/images/paint.jpeg'),
        content:'Instruction in the program is rooted in the investigation of painting as a unique genre with its own complex syntax and history. Within this setting, the program encourages diversity of practice and interpretation, innovation, and experimentation.',
        url:'#'
      },
      {
        title:'Photography',
        img: require('~/assets/images/photography.jpeg'),
        content:'Photography is a two-year program of study admitting ten students a year. Darkroom, studio, and computer facilities are provided. Students receive technical instruction in black-and-white and color photography as well as nonsilver processes and digital image production.',
        url:'#'
      },
      {
        title:'Sculpture',
        img: require('~/assets/images/sculpture.jpeg'),
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
