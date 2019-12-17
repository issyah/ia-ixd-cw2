<template>
    <div class="w-full px-4 py-0 bg-white relative z-50">
        <div class="container mx-auto md:flex justify-between items-center">
            <div class="items-center md:flex">
                <div class="py-2 md:py-0 flex justify-between md:flex-none">
                    <nuxt-link to="/">
                        <!-- <img src="~/assets/images/Yale_School_of_Art.png" alt="Yale School Of Art" class="h-3 block w-auto"/> -->
                        <div class="inline-block ml-2">
                            <span class="text-4xl font-semibold text-blue-800">YALE</span>
                        </div>
                    </nuxt-link>
                    <button class="md:hidden" @click="mobileNavHidden = !mobileNavHidden">
                        <svg class="fill-current w-4 h-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"></path></svg>
                    </button>
                </div>

                <div class="md:flex items-center justify-around" :class="{'hidden' : mobileNavHidden}">
                    <!-- Navigation -->
                    <div v-for="item in nav">
                        <template v-if="item.dropdown">
                            <div class="dropdown relative block md:inline-block mt-4 md:mt-0 md:pl-4">
                                <a href="#" class="text-gray-700 hover:text-gray-900 px-2 py-3 block md:inline-block border-b-4 border-transparent" :class="{'nav-links__active' : ($route.path.indexOf(item.activeLink)!= -1)}">{{item.title}}
                                    <svg viewBox="0 0 20 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="stroke-current inline w-3 y-3 text-black">
                                        <g id="Page-1" stroke="none" stroke-width="1" fill-rule="evenodd">
                                            <g id="icon-shape">
                                                <polygon id="Combined-Shape" points="9.29289322 12.9497475 10 13.6568542 15.6568542 8 14.2426407 6.58578644 10 10.8284271 5.75735931 6.58578644 4.34314575 8"></polygon>							</g>
                                            </g>
                                        </svg>
                                    </a>
                                    <div class="dropdown-menu rounded md:shadow-lg md:absolute md:w-56 md:left-0 md:bg-white md:hidden overflow-hidden py-2" v-if="!hideDropdown">
                                        <nuxt-link :key="index"  :to="dropdown.href" class="hover:text-gray-900 block px-4 py-2" :class="{'text-gray-900 font-semibold' : ($route.path.indexOf(dropdown.href)!= -1)}" v-for="(dropdown,index) in item.dropdown">{{dropdown.title}}</nuxt-link>
                                    </div>
                                </div>
                            </template>
                            <template v-else>
                                <div class="nav-links">
                                    <nuxt-link class="" :to="item.href" >{{item.title}}</nuxt-link>
                                </div>
                            </template>
                        </div>
                    </div>
                </div>
            <div class="md:flex items-center" :class="{'hidden' : mobileNavHidden}">
            <div class="nav-links">
                <a href="#" class="text-gray-600 hover:text-gray-900">Staff</a>
            </div>
            <div class="nav-links">
                <a href="#" class="text-gray-600 hover:text-gray-900">Students</a>
            </div>
        </div>
        </div>
    </div>
</template>
<style>
    .dropdown:hover  .dropdown-menu, .dropdown:focus .dropdown-menu{
        @apply block;
    }
    .dropdown:hover > a{
        @apply border-yellow-400;
    }
    .nav-links{
        @apply border-b-4 border-transparent px-2 py-3;
    }
    .nav-links:hover{
        @apply border-yellow-500;
    }
    .nav-links__active{
        @apply border-yellow-500 text-gray-900 font-semibold;
    }
</style>
<script>
    export default {
        data:()=>({
            mobileNavHidden: true,
            hideDropdown: false,
            nav: [
                {
                    title: 'About the School',
                    href:"",
                    dropdown:[
                        {title: 'Mission Statement', href:"#"},
                        {title: 'Visiting', href:"#"},
                        {title: 'About this Site', href:"#"}],
                        activeLink: 'about-the-school'
                },
                {title:'Admission', href:"", dropdown:[
                    {title: 'Graduate Programmes', href:"/admissions/graduate-programmes"},
                    {title: 'Financial Matters', href:"/admissions/financial-matters"}
                ],
                activeLink: 'admission'
                }
            ]
        }),
        mounted(){
        },
        watch:{
            $route(value){
                this.mobileNavHidden = true;
                // replicate on click href
                this.hideDropdown = true;
                setTimeout(()=>{this.hideDropdown = false},250);
            }
        }

    }
</script>
