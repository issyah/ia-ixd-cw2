<template>
  <div>
    <div class="w-full bg-gray-900 pb-10 pt-10 relative">
      <div class="absolute inset-0">
        <img src="~assets/images/graphic-design.jpg" alt="Graphic Design" class="w-full h-full absolute object-cover"/>
      </div>
      <!-- main content -->
      <div class="lg:w-9/12 mx-auto px-4 py-12 bg-gray-900 shadow-md -mb-40 relative">
        <div class="container mx-auto px-4 relative">
          <ul class="inline-block text-gray-600">
            <li class="inline">
              <nuxt-link to="/admissions/graduate-programmes" class="hover:text-yellow-400">Graduate Programme</nuxt-link>
            </li>
            <li class="inline">/</li>
            <li class="inline text-yellow-400">Graphic Design</li>
          </ul>
        </div>
        <div class="container mx-auto px-4 py-10 relative">
          <div class="text-center">
          </div>
          <div class="text-center">
            <div class="text-gray-400 font-bold text-xl">
              Masters Of Fine Arts
            </div>
            <div class="relative my-10 inline-block">
              <h1 class="text-6xl font-serif tracking-tight text-yellow-400 font-bold relative z-10">
                Graphic Design
              </h1>
              <div class="absolute bottom-0 h-5 w-full bg-gray-700 mb-2"></div>
            </div>
          </div>
        </div>
        <div class="md:w-3/4 lg:w-9/12 mx-auto">
          <h2 class="text-center text-3xl mb-4 text-gray-200 font-semibold">Programme Overview</h2>
          <p class="text-gray-400 text-lg leading-relaxed tracking-normal mb-2">The graphic design program focuses on the development of a cohesive, investigative body of work, also known as the student’s thesis. At Yale, the graphic design thesis is conceived as a loose framework within which each student’s visual method is deployed across many diverse projects during the two-year course of study. While every thesis project is unique, there are several common features: a focus on methodology, the application of a visual method to studio work, and the organization of the work in a thoughtfully argued written document and “Thesis Book.”</p>
          <p class="text-gray-400 text-lg leading-relaxed tracking-normal mb-2">
            The individual collection of graphic design work by each student is supported on several levels simultaneously: studio work led by faculty meeting weekly; small six-person thesis groups meeting biweekly; individual sessions with writing and editing tutors; and lectures, presentations, and workshops.
          </p>
          <div class="text-center mt-10 mb-10">
            <nuxt-link class="btn-programmes px-12" to="">
              Apply Now
            </nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div class="container mx-auto px-4 py-12 mt-40">
      <div class="md:w-4/5 lg:w-9/12 mx-auto">
        <h2 class="text-center text-3xl text-gray-800 mb-4 font-semibold">Facilities</h2>
        <p class="text-gray-700 text-lg leading-relaxed tracking-normal mb-2">
          The School of Art provides digital lab facilities however all graphic design students are expected to have their own personal computer. Each student has a designated work space in the design studio loft and has access to equipment including bookbinding materials, wide format printers, a RISO duplicator, Vandercook press, and work spaces in the School of Art buildings. More resources supporting interdisciplinary projects including motion capture and VR is available at the nearby Center for Collaborative Arts and Media. In addition, students draw on the extraordinary resources of Yale University courses, conferences, films, lectures, and museums, and especially the extensive research and rare book collections of Sterling, Haas, and Beinecke libraries.
        </p>

        <h2 class="text-center text-3xl text-gray-800 mt-8 mb-4 font-semibold">Two-year and preliminary-year programs</h2>
        <p class="text-gray-700 text-lg leading-relaxed tracking-normal mb-2">
          Each year, up to twelve students are admitted into the two-year graphic design program, and up to six students are admitted into the preliminary-year program. Two-year program students typically have a BFA in Graphic Design and are expected to have substantial and distinguished professional experience. Students applying to the preliminary-year program typically have relevant experience in a field of study outside design and demonstrate evidence of strong visual acuity. After successful completion of the preliminary year, these students automatically continue on in the two-year M.F.A. program.
        </p>
        <h2 class="text-center text-3xl text-gray-800 mt-8 mb-4 font-semibold">Credit Requirements</h2>
        <p class="text-gray-700 text-lg leading-relaxed tracking-normal mb-2">60 credits total are required to graduate. 42 credits in your area of concentration (including Art 949a, Critical Practice), and 18 additional credits, including a minimum of 6 academic credits which can be selected from throughout the University’s rich offerings.</p>
        <h2 class="text-center text-3xl text-gray-800 mt-8 mb-4 font-semibold">Programme Structure</h2>
        <!-- Accordion panels -->
        <!-- Prelim Year -->
        <div class="bg-white shadow rounded-lg mb-4">
          <div class="py-4 px-4 cursor-pointer flex justify-between items-center" @click="showPYear = !showPYear">
            <div>
              <div class="font-semibold">
                Preliminary-Year
              </div>
              <p class="text-gray-600">
                The preliminary year has a required studio course sequence and additional electives are not recommended.
              </p>
            </div>
            <div>
              <svg viewBox="0 0 20 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="stroke-current inline w-6 y-6 text-black">
                  <g id="Page-1" stroke="none" stroke-width="1" fill-rule="evenodd">
                    <g id="icon-shape">
                      <polygon id="Combined-Shape" points="9.29289322 12.9497475 10 13.6568542 15.6568542 8 14.2426407 6.58578644 10 10.8284271 5.75735931 6.58578644 4.34314575 8"></polygon>							</g>
                  </g>
              </svg>
            </div>
          </div>
          <div class="py-4 px-4" v-if="showPYear">
            <div class="mb-8">
              <h4 class="font-semibold text-lg">Fall</h4>
              <h5 class="text-gray-600">Total minimum Credits for fall term: <span class="font-bold text-gray-900">15</span></h5>
            </div>
            <div class="border border-gray-200 py-4 px-4 rounded">
              <table class="w-full text-left">
                <tr >
                  <th class="font-normal text-gray-500">ID</th>
                  <th class="font-normal text-gray-500">Title</th>
                  <th class="font-normal text-gray-500">Credits</th>
                </tr>
                <tr>
                  <td>Art 710a</td>
                  <td>Preliminary Studio</td>
                  <td>6</td>
                </tr>
                <tr>
                  <td>Art 264a2</td>
                  <td>Typography</td>
                  <td>3</td>
                </tr>
                <tr>
                  <td>Art 468a</td>
                  <td> Advanced Graphic Design: Series and System</td>
                  <td>3</td>
                </tr>
              </table>
            </div>
            <div class="my-8">
              <h4 class="font-semibold text-lg">Spring</h4>
              <h5 class="text-gray-600">Total minimum Credits for spring term: <span class="font-bold text-gray-900">15</span></h5>
            </div>
            <div class="border border-gray-200 py-4 px-4 rounded">
              <table class="w-full text-left">
                <tr >
                  <th class="font-normal text-gray-500">ID</th>
                  <th class="font-normal text-gray-500">Title</th>
                  <th class="font-normal text-gray-500">Credits</th>
                </tr>
                <tr>
                  <td>Art 711b</td>
                  <td>Preliminary Studio</td>
                  <td>6</td>
                </tr>
                <tr>
                  <td>Art 265b</td>
                  <td>Expression, Structure, and Sequence: Typography</td>
                  <td>3</td>
                </tr>
                <tr>
                  <td>Art 469b</td>
                  <td> Advanced Graphic Design: Series and System</td>
                  <td>3</td>
                </tr>
              </table>
            </div>
          </div>
        </div>
        <!-- First Year -->
        <div class="bg-white shadow rounded-lg mb-4">
          <div class="py-4 px-4 cursor-pointer flex justify-between items-center" @click="showFirstYear = !showFirstYear">
            <div>
              <div class="font-semibold">
                First year
              </div>
              <p class="text-gray-600">
                There are 3 required courses in the first year of the two-year program, totaling 15 credits. The remaining 15 credit requirements for the year must be fulfilled through a combination of studio and/or academic electives.
              </p>
            </div>
            <div>
              <svg viewBox="0 0 20 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="stroke-current inline w-6 y-6 text-black">
                  <g id="Page-1" stroke="none" stroke-width="1" fill-rule="evenodd">
                    <g id="icon-shape">
                      <polygon id="Combined-Shape" points="9.29289322 12.9497475 10 13.6568542 15.6568542 8 14.2426407 6.58578644 10 10.8284271 5.75735931 6.58578644 4.34314575 8"></polygon>							</g>
                  </g>
              </svg>
            </div>
          </div>
          <div class="py-4 px-4" v-if="showFirstYear">
            <div class="mb-8">
              <h4 class="font-semibold text-lg">Fall</h4>
              <h5 class="text-gray-600">Total minimum Credits for fall term: <span class="font-bold text-gray-900">15</span></h5>
            </div>
            <div class="text-gray-600">
              Required Courses:
            </div>
            <div class="border border-gray-200 py-4 px-4 rounded">
              <table class="w-full text-left">
                <tr >
                  <th class="font-normal text-gray-500">ID</th>
                  <th class="font-normal text-gray-500">Title</th>
                  <th class="font-normal text-gray-500">Credits</th>
                </tr>
                <tr>
                  <td>Art 720a</td>
                  <td>1st-year Graduate Studioo</td>
                  <td>6</td>
                </tr>
                <tr>
                  <td>Art 264a2</td>
                  <td>Typography</td>
                  <td>3</td>
                </tr>
                <tr>
                  <td>Art 468a</td>
                  <td> Advanced Graphic Design: Series and System</td>
                  <td>3</td>
                </tr>
              </table>
            </div>
            <div class="my-8">
              <h4 class="font-semibold text-lg">Spring</h4>
              <h5 class="text-gray-600">Total minimum Credits for spring term: <span class="font-bold text-gray-900">15</span></h5>
            </div>
            <div class="border border-gray-200 py-4 px-4 rounded">
              <table class="w-full text-left">
                <tr >
                  <th class="font-normal text-gray-500">ID</th>
                  <th class="font-normal text-gray-500">Title</th>
                  <th class="font-normal text-gray-500">Credits</th>
                </tr>
                <tr>
                  <td>Art 711b</td>
                  <td>Preliminary Studio</td>
                  <td>6</td>
                </tr>
                <tr>
                  <td>Art 265b</td>
                  <td>Expression, Structure, and Sequence: Typography</td>
                  <td>3</td>
                </tr>
                <tr>
                  <td>Art 469b</td>
                  <td> Advanced Graphic Design: Series and System</td>
                  <td>3</td>
                </tr>
              </table>
            </div>
          </div>
        </div>
        <!-- Second Year -->
        <div class="bg-white shadow rounded-lg">
          <div class="py-4 px-4 cursor-pointer flex justify-between items-center" @click="showSecondYear = ! showSecondYear">
            <div>
              <div class="font-semibold">
                Second year minimum credits
              </div>
              <p class="text-gray-600">
                There are 4 required courses in the second year of the two-year program, totaling 18 credits. The remaining 12 credit requirements for the year must be fulfilled through a combination of studio and/or academic electives.
              </p>
            </div>
            <div>
              <svg viewBox="0 0 20 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="stroke-current inline w-6 y-6 text-black">
                  <g id="Page-1" stroke="none" stroke-width="1" fill-rule="evenodd">
                    <g id="icon-shape">
                      <polygon id="Combined-Shape" points="9.29289322 12.9497475 10 13.6568542 15.6568542 8 14.2426407 6.58578644 10 10.8284271 5.75735931 6.58578644 4.34314575 8"></polygon>							</g>
                  </g>
              </svg>
            </div>
          </div>
          <div class="py-4 px-4" v-if="showSecondYear">
            <div class="mb-8">
              <h4 class="font-semibold text-lg">Fall</h4>
              <h5 class="text-gray-600">Total minimum Credits for fall term: <span class="font-bold text-gray-900">15</span></h5>
            </div>
            <div class="text-gray-600">
              Required Courses:
            </div>
            <div class="border border-gray-200 py-4 px-4 rounded">
              <table class="w-full text-left">
                <tr >
                  <th class="font-normal text-gray-500">ID</th>
                  <th class="font-normal text-gray-500">Title</th>
                  <th class="font-normal text-gray-500">Credits</th>
                </tr>
                <tr>
                  <td>Art 720a</td>
                  <td>1st-year Graduate Studioo</td>
                  <td>6</td>
                </tr>
                <tr>
                  <td>Art 264a2</td>
                  <td>Typography</td>
                  <td>3</td>
                </tr>
                <tr>
                  <td>Art 468a</td>
                  <td> Advanced Graphic Design: Series and System</td>
                  <td>3</td>
                </tr>
              </table>
            </div>
            <div class="my-8">
              <h4 class="font-semibold text-lg">Spring</h4>
              <h5 class="text-gray-600">Total minimum Credits for spring term: <span class="font-bold text-gray-900">15</span></h5>
            </div>
            <div class="border border-gray-200 py-4 px-4 rounded">
              <table class="w-full text-left">
                <tr >
                  <th class="font-normal text-gray-500">ID</th>
                  <th class="font-normal text-gray-500">Title</th>
                  <th class="font-normal text-gray-500">Credits</th>
                </tr>
                <tr>
                  <td>Art 711b</td>
                  <td>Preliminary Studio</td>
                  <td>6</td>
                </tr>
                <tr>
                  <td>Art 265b</td>
                  <td>Expression, Structure, and Sequence: Typography</td>
                  <td>3</td>
                </tr>
                <tr>
                  <td>Art 469b</td>
                  <td> Advanced Graphic Design: Series and System</td>
                  <td>3</td>
                </tr>
              </table>
            </div>
          </div>
        </div>

        <div class="text-center mt-24">
          <nuxt-link class="px-16 py-4 text-lg font-semibold shadow text-yellow-900 bg-yellow-500 rounded-full text-white hover:shadow-lg" to="">
            APPLY NOW
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
.btn-programmes{
  @apply py-2 px-24 rounded-full border-2 border-yellow-400 text-yellow-400 inline-block
}
.btn-programmes:hover{
  @apply bg-yellow-400 text-gray-900
}
</style>
<script>
  export default{
    data:()=>({
      showPYear: false,
      showFirstYear:false,
      showSecondYear: false,
    }),
    head(){
      return{
        title:'Graphic Design - Yale School Of Arts'
      }
    }
  }
</script>
