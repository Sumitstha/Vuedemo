
<template>
    <div>
 
   <header>
    <nav class=" bg-gray-900 px-3 py-3 shadow text-gray-400 flex justify-between ">
    
          <div class=" ">
        <span class="text-2xl font-[Poppins] cursor-pointer">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5vjfJanFsa9sLPzuhAtjLuUKTen37v4JNUA&usqp=CAU" class="h-6 inline mb-2 rounded-lg">
            <p class="inline mx-4 text-slate-50 text-2xl font-bold font-serif">Tailwind</p>
        </span>
      
        </div>

      <div>
<ul class=" md:flex md:items-center z-[-1] md:z-auto md:static absolute w-full left-0 md:w-auto md:py-0 py-4 md:pl-0 pl-7 md:opacity-100 opacity-0 top=[-400px] transition-all ease-in duration-500">

<li class="mx-2 my-2 md:my-0">
        
       <button @click="open=!open" id="dropdownbtn" data-dropdown-toggle="dropdown" class=" relative text-base hover:text-white duration-100 font-semibold mx-2" type="button "><span><i class="fa-solid fa-house-crack mr-1"></i></span>Dashboards

        <svg class="w-4 h-4 ml-3 inline" aria-hidden="true" fill="none" stroke="currentColor" viewBox="0 0 24 24" ><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M18 9l-7 7-7-7"></path></svg>

        </button>

<div v-if="open" id="dropdown" class=" absolute z-10  bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700">
<ul class="py-2 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="dropdownDefaultButton">
  <li>
    
    <a href="#" @click="$router.push({name:'home'})" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Analytics</a>
  </li>
  <li>
    <a href="#" @click="$router.push({name:'ecom'})" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Ecommerce</a>
  </li>
  <li>
    <a href="#" @click="$router.push({name:'project'})" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Project</a>
  </li>
  <li>
    <a href="" @click="$router.push({name:'nft'})" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">NFTs</a>
  </li>
  
</ul>
</div>
</li>


<li class="mx-2 my-2 md:my-0">
        <button id="dropdownbtn" data-dropdown-toggle="dropdown" class="text-base hover:text-white duration-100 font-semibold mx-1" type="button"><span><i class="fa-solid fa-tablet-screen-button mr-1"></i></span>Apps
            <svg class="w-4 h-4 ml-1 inline" aria-hidden="true" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path></svg>
        </button></li>

        <li class="mx-2 my-2 md:my-0">
        <button id="dropdownbtn" data-dropdown-toggle="dropdown" class="text-base hover:text-white duration-100 font-semibold mx-1" type="button"><span><i class="fa-solid fa-globe mr-1"></i></span>UI Kit
            <svg class="w-4 h-4 ml-1 inline" aria-hidden="true" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path></svg>
        </button></li>

        <li class="mx-2 my-2 md:my-0">
        <button id="dropdownbtn" data-dropdown-toggle="dropdown" class="text-base hover:text-white duration-100 font-semibold mx-2" type="button"> <span><i class="fa-regular fa-file-lines mr-1"></i></span>Pages
            <svg class="w-4 h-4 ml-1 inline" aria-hidden="true" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path></svg>
        </button></li>
        
     <li class="mx-2 my-2 md:my-0">
        <button id="dropdownbtn" data-dropdown-toggle="dropdown" class="text-base hover:text-white duration-100 font-semibold " type="button"><span><i class="fa-solid fa-shield-halved mr-1"></i></span>Authentication
            <svg class="w-4 h-4 ml-1 inline" aria-hidden="true" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path></svg>
        </button></li>
    </ul>
  </div> 

       
       <div class="relative flex items-center text-white  ">
        
       <!-- <SearchIcon class=" h-5 w-5 absolute ml-3"/> -->
       <i class="fa-solid fa-magnifying-glass h-5 w-5 absolute ml-4 mt-1"></i>
        <input type="text" id="searchbar" class="  rounded-lg border border-gray-700 bg-gray-900 p-2 pl-10 text-gray-300 outline-none sm:text-sm focus-within:text-gray-900 " placeholder="Search...">
       </div>
       <div class="float-right md:inline-block">
        
        <button @click="open1=!open1" id="dropdownbtn" data-dropdown-toggle="dropdown" class=" relative text-base hover:text-white duration-100 font-semibold mx-2 " type="button">
            <img v-bind:src=" productImage " class="h-6 inline rounded-xl ">

         </button>

<div v-if="open1" id="dropdown" class=" absolute z-10  bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700">
 <ul class="py-2 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="dropdownDefaultButton">
   <li>
     
     <a href="" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Dashboard</a>
   </li>
   <li>
     <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Setting</a>
   </li>
   <li>
     <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Earning</a>
   </li>
   <li>
     <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Signout</a>
   </li>
   
 </ul>
</div>
</div>

</nav>
</header>
<main>
        <slot>

        </slot>
    </main>
    <footer ></footer>
    

</div>

</template>

<script>
//  import {SearchIcon} from "@heroicons/vue/outline/index";
   
export default {
   
    name:'NavBar',
    data(){
        return{
            open:false,
            open1:false,
            productImage:require("../assets/images/avatar-1.jpg"),
            components:{}
        }
    },

    }
   


</script>