<template>
<body class="font-[Poppins] bg-gradient-to-t from-slate-50 to-slate-200 h-auto">
    <div class="container mx-auto bg-slate-100">
        <div class="flex flex-wrap ">
            <div class="flex items-center px-4 py-2 w-full">
                <div class="w-full">
                    <div class="flex justify-between">
                        <div>
                            <h1 class="font-semibold block font-2xl">Dashboard</h1>
                            <ol class="flex ">
                                <li>T-Wind</li>
                                <li class="px-1"><span>/</span></li>
                                <li class="px-1">Dashboard</li>
                                <li class="px-1"><span>/</span></li>
                                <li class="text-blue-500 hover:text-blue-600 px-1">Project</li>
                            </ol>
                        </div>
                        <div class="flex items-center">
                            <div>
                                <button class="bg-blue-600 hover:bg-blue-700 px-4 py-1 rounded-lg text-white">Create New</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- start of the boxes -->

        <div id="top" class=" flex justify-between bg-gray-100  mx-2">

            <div id="div1" class=" rounded-md shadow h-20 w-full pt-2  m-2  bg-white ">
                <div class="flex justify-between relative">
                    <div>
                        <p class="text-slate-400 font-medium mt-1 ml-4">PROJECTS</p>
                        <h3 class=" font-semibold text-2xl mt-1 ml-6">78</h3>
                    </div>
                    <div><span><i class="fa-solid fa-ellipsis-vertical text-gray-500 mt-6 mr-6"></i></span></div>

                </div>
            </div>
            <div id="div2" class="shadow rounded-md  h-20 w-full pt-2 m-2 bg-white">
                <div class="flex justify-between relative">
                    <div>
                        <p class="text-slate-400 font-medium mt-1 ml-4">TASKS</p>
                        <div class="flex">
                            <h3 class=" font-semibold text-2xl mt-1 ml-6">40</h3>
                            <span class=" rounded-sm ml-2 mt-2 mb-2 bg-green-300"><small class="  text-green-800">Active</small></span>
                        </div>
                    </div>
                    <div><span><i class="fa-solid fa-diagram-predecessor  text-gray-500 mt-6 mr-6"></i></span></div>
                </div>

            </div>

            <div id="div3" class=" shadow rounded-md h-20 w-full pt-2 m-2 bg-white">
                <div class="flex justify-between relative">
                    <div>
                        <p class="text-slate-400 font-medium mt-1 ml-4">TOTAL HOURS</p>
                        <h3 class=" font-semibold text-2xl mt-1 ml-6">24k</h3>
                    </div>
                    <div><span><i class="fa-regular fa-clock  text-gray-500 mt-6 mr-6"></i></span></div>
                </div>
            </div>
            <div id="div4" class=" rounded-md shadow h-20 w-full pt-2 m-2  bg-white">
                <div class="flex justify-between relative">
                    <div>
                        <p class="text-slate-400 font-medium mt-1 ml-4">BUDGET</p>
                        <h3 class=" font-semibold text-2xl mt-1 ml-6">$24100</h3>
                    </div>
                    <div><span><i class="fa-solid fa-dollar-sign  text-gray-500 mt-6 mr-6"></i></span></div>
                </div>
            </div>
        </div>

        <!-- middle part -->
        <div id="two" class="flex justify-between mx-2 bg-gray-100">

            <div id="d1" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Task Performance</h1>
                    </div>
                    <hr />
                </div>
                <div class="p-5">
                    <img :src="char" alt="oop" class="h-60" />
                </div>

            </div>

            <div id="d2" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div class="pt-4"></div>

                <canvas id="mycart" class=" h-full  m-6 pb-6 pl-6 pr-16 pt-6 "></canvas>
                <div class="pb-4"></div>

            </div>
            <div id="d3" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div class="text-center ">
                    <div class="flex justify-center">
                        <img :src="deer" alt="deer" class="rounded-full  h-24" />
                    </div>

                    <h3 class=" font-semibold text-2xl mt-1 ml-6">Management System</h3>
                    <p class="text-slate-400 font-medium mt-1 ml-4"><small> #123658</small></p>
                </div>

                <div class=" ">
                    <input type="checkbox" class="form-checkbox  ml-4 h-4 w-4 text-indigo-600" v-model="isChecked">
                    <label for="checkbox" class="ml-2 font-bold">Planning</label><br>
                    <input type="checkbox" class="form-checkbox ml-4 h-4 w-4 text-indigo-600" v-model="Checked">
                    <label for="checkbox" class="ml-2 font-bold">Design</label><br>

                    <input type="checkbox" class="form-checkbox ml-4 h-4 w-4 text-indigo-600" v-model="hecked">
                    <label for="checkbox" class="ml-2 font-bold">Testing</label><br>

                </div>

                <div class=" flex items-center p-2 mb-4">
                    <div class="w-full relative bg-gray-500 h-2 rounded-full mx-5">
                        <div class="h-2 w-2/3  bg-blue-500 rounded-full"></div>
                    </div>

                </div>

                <div class="border-b border-dashed border-slate-200 dark:border-slate-700">

                </div>
                <div class="flex justify-between py-1">
                    <div class="flex">
                        <img :src="a2" alt="a2" class="rounded-full h-8 mx-auto hover:z-10 cursor-pointer ml-4 " />
                        <img :src="a3" alt="a3" class="rounded-full h-8 mx-auto hover:z-10 cursor-pointer -ml-4" />
                        <img :src="a4" alt="a4" class="rounded-full h-8 mx-auto hover:z-10 cursor-pointer -ml-4" />
                        <img :src="a5" alt="a5" class="rounded-full h-8 mx-auto hover:z-10 cursor-pointer -ml-4" />
                        <img :src="a6" alt="a6" class="rounded-full h-8 mx-auto hover:z-10 cursor-pointer -ml-4" />
                        <img :src="a7" alt="a7" class="rounded-full h-8 mx-auto hover:z-10 cursor-pointer -ml-4" />

                    </div>
                    <div>
                        <button class=" hover:bg-blue-700 hover:text-black bg-gray-300 px-4 py-1 rounded-sm mr-4 text-blue-700">More Details</button>
                    </div>

                </div>

            </div>

        </div>

        <!-- last part -->

        <div id="last" class=" flex justify-between overflow-y-auto min-w-full mt-4 bg-gray-100  ">

            <div id="da1" class=" w-full  ml-1">
                <div id="ek" class="flex justify-start w-full mx-auto">
                    <div>
                        <h1 class="font-bold">MEETING</h1>
                        <p>3 Issues - <span class="text-slate-400">20 Points</span></p>

                    </div>

                </div>
                <div class="border-b border-pink-600  "></div>
                <div id="div1" class=" rounded-md shadow h-30 w-full pt-2 mt-2  bg-white ">

                    <div id="dui" class=" p-2">
                        <span class=" bg-green-200 text-green-900 rounded-sm p-1 "><small>Mobile App</small></span>
                        <h4>Mobile Account Setting</h4>
                        <p class="text-slate-400">Contrary to popular belief, Lorem Ipsum is not simply random text.</p>
                        <div class="border-b border-dashed border-slate-200 dark:border-slate-700 my-4"></div>

                    </div>

                    <div id="teen" class="flex justify-between p-2">
                        <div class="flex ">

                            <p> <span><i class="fa-solid fa-paperclip"></i></span> 6</p>
                            <p class="ml-2"><i class="fa-regular fa-comment"></i>3</p>

                        </div>
                        <div class="flex">

                            <img :src="a2" alt="a2" class="rounded-full h-8  hover:z-10 cursor-pointer  " />
                            <img :src="a3" alt="a3" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                            <img :src="a4" alt="a4" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                        </div>

                    </div>
                </div>
                <div id="div1" class=" rounded-md shadow h-30 w-full pt-2  mt-2   bg-white ">

                    <div id="dui" class=" p-2">
                        <span class=" bg-blue-200 text-blue-900 rounded-sm p-1 "><small>UI/UX</small></span>
                        <h4>Dribble Shot</h4>
                        <img :src="il" alt="il" class="h-30  " />
                        <div class="border-b border-dashed border-slate-200 dark:border-slate-700 my-4"></div>

                    </div>

                    <div id="teen" class="flex justify-between p-2">
                        <div class="flex ">

                          <p> <span><i class="fa-solid fa-paperclip"></i></span> 6</p>
                            <p class="ml-2"><i class="fa-regular fa-comment"></i>3</p>

                        </div>
                        <div class="flex">

                            <img :src="a4" alt="a4" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                        </div>

                    </div>
                </div>

            </div>

            <div id="da2" class=" w-full  mx-2">
                <div id="ek" class="flex justify-start w-full mx-auto">
                    <div>
                        <h1 class="font-bold">TODO</h1>
                        <p>3 Issues - <span class="text-slate-400">20 Points</span></p>

                    </div>

                </div>
                <div class="border-b border-green-600 "></div>
                <div id="div1" class=" rounded-md shadow h-30 w-full pt-2  mt-2   bg-white ">

                    <div id="dui" class=" p-2">
                        <span class=" bg-yellow-200 text-yellow-900 rounded-sm p-1 "><small>Pharma Web</small></span>
                        <h4>Covid Vaccine</h4>
                        <p class="text-slate-400">Contrary to popular belief, Lorem Ipsum is not simply random text.</p>
                        <div class="border-b border-dashed border-slate-200 dark:border-slate-700 my-4"></div>

                    </div>

                    <div id="teen" class="flex justify-between p-2">
                        <div class="flex ">

                            <p> <span><i class="fa-solid fa-paperclip"></i></span> 6</p>
                            <p class="ml-2"><i class="fa-regular fa-comment"></i>3</p>

                        </div>
                        <div class="flex">

              
                            <img :src="a4" alt="a4" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                        </div>

                    </div>
                </div>
                <div id="div1" class=" rounded-md shadow h-30 w-full pt-2  mt-2   bg-white ">

                    <div id="dui" class=" p-2">
                        <span class=" bg-purple-200 text-purple-900 rounded-sm p-1 "><small>UI/UX</small></span>
                        <h4>Dribble Shot</h4>
                        <p class="text-slate-400">The adventurous explorers hiked through the dense jungle, encountering exotic wildlife along the way.</p>



                        
                        <div class="border-b border-dashed border-slate-200 dark:border-slate-700 my-4"></div>

                    </div>

                    <div id="teen" class="flex justify-between p-2">
                        <div class="flex ">

                          <p> <span><i class="fa-solid fa-paperclip"></i></span> 6</p>
                            <p class="ml-2"><i class="fa-regular fa-comment"></i>3</p>

                        </div>
                        <div class="flex">

                          <img :src="a2" alt="a2" class="rounded-full h-8  hover:z-10 cursor-pointer  " />
                           
                        </div>

                    </div>
                </div>

            </div>

            <div id="da3" class=" w-full  mx-2">
                <div id="ek" class="flex justify-start w-full mx-auto">
                    <div>
                        <h1 class="font-bold">IN PROGRESS</h1>
                        <p>3 Issues - <span class="text-slate-400">20 Points</span></p>

                    </div>

                </div>
                <div class="border-b border-blue-600 "></div>
                <div id="div1" class=" rounded-md shadow h-30 w-full pt-2  mt-2   bg-white ">

                    <div id="dui" class=" p-2">
                        <span class=" bg-pink-200 text-pink-900 rounded-sm p-1 "><small>UI/UX</small></span>
                        <h4>Dribble Shot</h4>
                        <img :src="il1" alt="il1" class="h-30  " />
                        <div class="border-b border-dashed border-slate-200 dark:border-slate-700 my-4"></div>

                    </div>

                    <div id="teen" class="flex justify-between p-2">
                        <div class="flex ">

                            <p> <span><i class="fa-solid fa-paperclip"></i></span> 6</p>
                            <p class="ml-2"><i class="fa-regular fa-comment"></i>3</p>

                        </div>
                        <div class="flex">

                            <img :src="a2" alt="a2" class="rounded-full h-8  hover:z-10 cursor-pointer  " />
                           
                            
                        </div>

                    </div>
                </div>
                <div id="div1" class=" rounded-md shadow h-30 w-full pt-2  mt-2   bg-white ">

                    <div id="dui" class=" p-2">
                        <span class=" bg-green-200 text-green-900 rounded-sm p-1 "><small>UI/UX</small></span>
                        <h4>Dribble Shot</h4>
                        <img :src="il" alt="il" class="h-30  " />
                        <div class="border-b border-dashed border-slate-200 dark:border-slate-700 my-4"></div>

                    </div>

                    <div id="teen" class="flex justify-between p-2">
                        <div class="flex ">

                          <p> <span><i class="fa-solid fa-paperclip"></i></span> 6</p>
                            <p class="ml-2"><i class="fa-regular fa-comment"></i>3</p>

                        </div>
                        <div class="flex">

                            <img :src="a4" alt="a4" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                        </div>

                    </div>
                </div>

            </div>

            <div id="da4" class=" w-full  mx-2">
                <div id="ek" class="flex justify-start w-full mx-auto">
                    <div>
                        <h1 class="font-bold">TESTING</h1>
                        <p>3 Issues - <span class="text-slate-400">20 Points</span></p>

                    </div>

                </div>
                <div class="border-b border-red-600 "></div>
                <div id="div1" class=" rounded-md shadow h-30 w-full pt-2  mt-2   bg-white ">

                    <div id="dui" class=" p-2">
                        <span class=" bg-blue-200 text-blue-900 rounded-sm p-1 "><small>Mobile App</small></span>
                        <h4>Mobile Account Setting</h4>
                        <p class="text-slate-400">Contrary to popular belief, Lorem Ipsum is not simply random text.</p>
                        <div class="border-b border-dashed border-slate-200 dark:border-slate-700 my-4"></div>

                    </div>

                    <div id="teen" class="flex justify-between p-2">
                        <div class="flex ">

                            <p> <span><i class="fa-solid fa-paperclip"></i></span> 6</p>
                            <p class="ml-2"><i class="fa-regular fa-comment"></i>3</p>

                        </div>
                        <div class="flex">

                            <img :src="a2" alt="a2" class="rounded-full h-8  hover:z-10 cursor-pointer  " />
                            <img :src="a3" alt="a3" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                            <img :src="a4" alt="a4" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                        </div>

                    </div>
                </div>
                <div id="div1" class=" rounded-md shadow h-30 w-full pt-2  mt-2   bg-white ">

                    <div id="dui" class=" p-2">
                        <span class=" bg-red-200 text-red-900 rounded-sm p-1 "><small>UI/UX</small></span>
                        <h4>Dribble Shot</h4>
                        <img :src="il" alt="il" class="h-30  " />
                        <div class="border-b border-dashed border-slate-200 dark:border-slate-700 my-4"></div>

                    </div>

                    <div id="teen" class="flex justify-between p-2">
                        <div class="flex ">

                          <p> <span><i class="fa-solid fa-paperclip"></i></span> 6</p>
                            <p class="ml-2"><i class="fa-regular fa-comment"></i>3</p>

                        </div>
                        <div class="flex">

                            <img :src="a4" alt="a4" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                        </div>

                    </div>
                </div>

            </div>

            <div id="da5" class=" w-full  mx-2">
                <div id="ek" class="flex justify-start w-full mx-auto">
                    <div>
                        <h1 class="font-bold">DONE</h1>
                        <p>3 Issues - <span class="text-slate-400">20 Points</span></p>

                    </div>

                </div>
                <div class="border-b border-yellow-600 "></div>
                <div id="div1" class=" rounded-md shadow h-30 w-full pt-2  mt-2   bg-white ">

                    <div id="dui" class=" p-2">
                        <span class=" bg-green-200 text-green-900 rounded-sm p-1 "><small>Mobile App</small></span>
                        <h4>Mobile Account Setting</h4>
                        <p class="text-slate-400">With a burst of laughter, friends gathered around the bonfire, sharing stories and making memories.</p>
                        <div class="border-b border-dashed border-slate-200 dark:border-slate-700 my-4"></div>

                    </div>

                    <div id="teen" class="flex justify-between p-2">
                        <div class="flex ">

                            <p> <span><i class="fa-solid fa-paperclip"></i></span> 6</p>
                            <p class="ml-2"><i class="fa-regular fa-comment"></i>3</p>

                        </div>
                        <div class="flex">

                            <img :src="a2" alt="a2" class="rounded-full h-8  hover:z-10 cursor-pointer  " />
                            <img :src="a3" alt="a3" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                            <img :src="a4" alt="a4" class="rounded-full h-8  hover:z-10 cursor-pointer ml-2 " />
                        </div>

                    </div>
                </div>
                

            </div>

        </div>


    </div>

</body>
</template>

<script>
//   import LayoutView from './LayoutView.vue';
import Chart from 'chart.js/auto';
export default {
    //   components:{LayoutView}
    data() {
        return {
            isChecked: false,
            Checked: false,
            hecked: false,
            char: require('@/assets/images/gol.png'),
            deer: require('@/assets/images/p1.png'),
            a2: require('@/assets/users/avatar-2.jpg'),
            a3: require('@/assets/users/avatar-3.jpg'),
            a4: require('@/assets/users/avatar-4.jpg'),
            a5: require('@/assets/users/avatar-5.jpg'),
            a6: require('@/assets/users/avatar-6.jpg'),
            a7: require('@/assets/users/avatar-7.jpg'),
            il: require('@/assets/users/ill-2.png'),
            il1: require('@/assets/users/ill-1.png'),
        }
    },
    mounted() {
        console.log('component mounted.')
        const ctx = document.getElementById('mycart');
        const myCart = new Chart(ctx, {
            type: 'bar',
            data: {
                labels: ['Red', 'Orange', 'Yellow', 'Green', 'Blue', 'Purple', 'Cyan', 'Teal', 'Black', 'brown'],
                datasets: [{
                    label: '# of Votes',
                    data: [12, 19, 3, 5, 2, 3, 8, 10, 6, 10],
                    backgroundColor: [
                        'rgba(255, 99, 132, 0.2)',
                        'rgba(255, 159, 64, 0.2)',
                        'rgba(255, 205, 86, 0.2)',
                        'rgba(75, 192, 192, 0.2)',
                        'rgba(54, 162, 235, 0.2)',
                        'rgba(153, 102, 255, 0.2)',
                        'rgba(201, 203, 207, 0.2)',
                        'rgba(0, 255, 255, 0.2)',
                        'rgb(0, 0, 0,0.2)',
                        'rgba(127, 255, 212, 0.2)',
                        'rgba(139, 69, 19, 0.2)',

                    ],
                    borderColor: [
                        'rgb(255, 99, 132)',
                        'rgb(255, 159, 64)',
                        'rgb(255, 205, 86)',
                        'rgb(75, 192, 192)',
                        'rgb(54, 162, 235)',
                        'rgb(153, 102, 255)',
                        'rgb(201, 203, 207)',
                        'rgb(0, 255, 255)',
                        'rgb(0, 0, 0)',
                        'rgb(127, 255, 212)',
                        'rgb(139, 69, 19)',
                    ],
                    borderWidth: 4
                }]
            },
            options: {
                scales: {
                    y: {
                        beginAtZero: true
                    }
                }
            }
        });
        myCart;
    },
}
</script>

<style >

  </style>
