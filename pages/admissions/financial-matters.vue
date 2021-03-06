<template>
  <div>
    <div class="bg-gray-900 py-4">
        <div class="container px-4 mx-auto">
          <!-- heading -->
          <div class="relative inline-block">
            <h1 class="text-5xl font-serif tracking-tight text-yellow-400 font-bold relative z-10">
              Financial Matters
            </h1>
            <div class="absolute bottom-0 h-5 w-full bg-gray-700 mb-2"></div>
          </div>

        </div>
    </div>

    <div class="container px-4 mx-auto">
      <!-- Main Tab Section -->
      <div class="my-10">
        <ul class="inline-block">
          <li class="inline">
            <a href="javascript:;" class="finance__tab_li" :class="setActive('tuition')" @click="tab = 'tuition'">Tuition Fees</a>
          </li>
          <li class="inline">
            <a href="javascript:;" class="finance__tab_li" :class="setActive('scholarship')" @click="tab = 'scholarship'">Scholarship</a>
          </li>
          <li class="inline">
            <a href="javascript:;" class="finance__tab_li" :class="setActive('loans')" @click="tab = 'loans'">Loans</a>
          </li>
        </ul>
      </div>

      <!-- Main Content Section -->
      <div class="container mx-auto my-10 ">
        <div class="py-4 px-10 bg-white">
          <template v-if="tab == 'tuition'">
            <div>
              <h3 class="text-2xl font-semibold mt-10">Tuition Fees</h3>
              <h2 class="text-4xl font-bold font-serif text-gray-700">$39,924</h2>
              <p class="mt-4 leading-relaxed text-gray-900">
                The tuition fee for the academic year 2019-2020 is $39,924. The Corporation of Yale University reserves the right to revise tuition rates as necessary.
              </p>
            </div>

            <div>
              <h3 class="text-2xl font-semibold mt-10">Cost Of Attendance</h3>
              <h2 class="text-4xl font-bold font-serif text-gray-700">$17,756</h2>
              <p class="mt-4 leading-relaxed text-gray-900">
                The student budget includes an amount for tuition, books, and supplies, estimated living expenses, and Yale Health Plan coverage costs. The living expense budget for the 2019-2020 academic year (Sept- May) is $17,756. In other words, it is assumed that students at Yale School of Art can cover the cost of housing, utilities, food, health services, clothing and laundry, miscellaneous items, and in-school travel within a total budget of approximately $1,972 per month. It is expected that you will spend the greater part of your time in academic work; therefore, it is assumed that your lifestyle will be one appropriate to that of a fulltime student. To this end, you should be prepared to economize during your time here.
              </p>
            </div>

            <div>
              <h3 class="text-2xl font-semibold mt-10">Other Fees</h3>
              <div class="flex items-center">
                <span class="text-4xl font-bold font-serif text-gray-700">$2,402</span>  &nbsp;  - <span class="text-gray-600">hospitalisation insurance, est (single student)</span>
              </div>
              <p class="mt-4 leading-relaxed text-gray-900">
                The following fees are charged each year to the Student Financial Services bill for use of and/or access to special facilities; this is a uniform mandatory fee that is refundable only upon withdrawal from the program, according to the tuition rebate schedule.
              </p>
            </div>
          </template>
          <!-- Scholarship -->
          <template v-if="tab == 'scholarship'">
            <h3 class="text-2xl font-semibold mt-10">
              Scholarship
            </h3>
            <p class="mt-4 leading-relaxed text-gray-900">
              When the total amount of the student contribution, parent contribution, employment/work-study and loans do not meet a student’s full financial need, scholarship funds are awarded. Scholarships are also known as grant or gift aid and, unlike loans, do not have to be repaid. If your financial aid applications are received and processed by the School’s deadline and you have calculated need, the School makes every effort to award a substantial scholarship to you. Scholarship availability is based on the number of students with calculated financial need within the School and the amount of funds available.
            </p>
            <p class="mt-4 leading-relaxed text-gray-900">
              Scholarship is need-based and only awarded to accepted students who’ve applied for aid and have demonstrated need. The maximum scholarship for first-year students does not exceed tuition costs.
            </p>
          </template>

          <!-- Loans -->
          <template v-if="tab == 'loans'">
            <h3 class="text-2xl font-semibold mt-10">
              Loans
            </h3>
            <p class="mt-4 leading-relaxed text-gray-900">
              A portion of your financial need will be met with an offer of a unit loan. Your loan offer is composed of loans from either the Federal Direct Loan Programs if you are a U.S. Citizen/Permanent Resident or an alternative/private bank/Yale International Student loan if you do not qualify for the federal loan programs or you are an International Student. You must indicate the type and amount of the loan you would like to borrow, if you choose to borrow, on the Art Loan Form 2019-20.
            </p>
          </template>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
  .finance__tab_li{
    @apply px-4 py-2 bg-white rounded-full mx-2 inline-block mt-2;
  }
  .finance__tab_li.active{
    @apply bg-yellow-400 shadow-lg font-semibold text-yellow-900;
  }
</style>
<script>
  export default {
    data:() =>({
      tab: 'tuition'
    }),
    methods:{
      setActive(tab){
        if(tab == this.tab){
          return 'active';
        }
      }
    },
    head:() =>({
      title: 'Financial Matters - Yale School of Arts'
    })
  }
</script>
