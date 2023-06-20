<template>
<body class="font-[Poppins] bg-gradient-to-t from-slate-50 to-slate-200 h-auto">
    <div class="container mx-auto bg-slate-100">
        <div class="flex flex-wrap">
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
                                <li class="text-blue-500 hover:text-blue-600 px-1">Nft</li>
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

        <!-- start -->
        <div id="top" class="flex justify-between mx-2 bg-gray-100">

            <div id="d1" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div class="text-center ">

                    <img :src="staticData[0].bg" alt="bg" class="h-full p-2" />

                    <div class=" flex justify-center -mt-10">
                        <img :src="staticData[0].mon" alt="mon" class="rounded-full h-20" />
                    </div>
                    <h3 class=" font-semibold text-2xl mt-1 ml-6">T-Wind#309</h3>
                    <p class="text-slate-400 font-medium mt-1 ml-4"><small> @Martin Gibson</small></p>
                </div>

                <div class=" flex justify-between pb-2 pt-2 bg-white">
                    <div class="border-r border-dashed  border-b  border-t w-full pt-2  bg-white">
                        <div class=" text-center">
                            <h1 class="font-mono text-slate-400  dark:text-slate-300 "><small>Current Bid</small>

                            </h1>
                            <h2 class="font-mono text-xl  font-semibold">1.55 ETH
                            </h2>
                        </div>
                    </div>
                    <div class="border-r border-dashed  border-b border-t  w-full pt-2  bg-white">
                        <div class=" text-center">
                            <h1 class="font-mono text-slate-400   dark:text-slate-300 "><small> Auction Duration</small>

                            </h1>
                            <h2 class="font-mono text-xl   font-semibold">0 0 0 0</h2>
                        </div>
                    </div>
                </div>
                <div class="pb-2 text-center">
                    <button class="bg-blue-600 hover:bg-blue-700 px-6 py-1  rounded-lg text-white">Start Auction</button>
                </div>

            </div>

            <div id="d2" class="  h-full w-full  m-2 ">
                <div id="d2-1" class="bg-white rounded-md mb-4">
                    <img :src="staticData[0].boa" alt="boa" class="h-full pt-16 pb-16 ml-4" />
                </div>

                <div id="d2-2" class=" rounded-md my-2 flex justify-between">
                    <div id="div3" class=" shadow rounded-md h-20 w-full pt-2 m-2 bg-white">
                        <div class="flex justify-between relative">
                            <div><span><i class="fa-solid fa-dollar-sign   text-gray-500 mt-6 ml-6"></i></span></div>
                            <div>
                                <h3 class=" font-semibold text-2xl mt-1 mr-6">$24948</h3>
                                <p class="text-slate-400 font-medium mt-1 mr-4">Revenue</p>

                            </div>

                        </div>
                    </div>
                    <div id="div4" class=" rounded-md shadow h-20 w-full pt-2 m-2  bg-white">
                        <div class="flex justify-between relative">
                            <div><span><i class="fa-brands fa-ethereum  text-gray-500 mt-6 ml-6"></i></span></div>
                            <div>
                                <h3 class=" font-semibold text-2xl mt-1 mr-6">+12.3%</h3>
                                <p class="text-slate-400 font-medium mt-1 mr-4">ROI</p>

                            </div>
                        </div>
                    </div>
                </div>

                <div id="d2-3" class="rounded-md my-2 flex justify-between">
                    <div id="div3" class=" shadow rounded-md h-20 w-full pt-2 m-2 bg-white">
                        <div class="flex justify-between relative">
                            <div><span><i class="fa-brands fa-nfc-symbol text-gray-500 mt-6 ml-6"></i></span></div>
                            <div>
                                <h3 class=" font-semibold text-2xl mt-1 mr-6">12.33</h3>
                                <p class="text-slate-400 font-medium mt-1 mr-4">Spending</p>

                            </div>
                        </div>
                    </div>
                    <div id="div4" class=" rounded-md shadow h-20 w-full pt-2 m-2  bg-white">
                        <div class="flex justify-between relative">
                            <div><span><i class="fa-solid fa-arrows-up-to-line text-gray-500 mt-6 ml-6"></i></span></div>
                            <div>
                                <h3 class=" font-semibold text-2xl mt-1 mr-6">24.44</h3>
                                <p class="text-slate-400 font-medium mt-1 mr-4">Estimated</p>

                            </div>
                        </div>
                    </div>
                </div>

            </div>

            <div id="d3" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div class="py-6">
                    <div class="card-header pb-6">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Task Performance</h1>
                    </div>
                    <hr />
                </div>
                <div class="p-5">
                    <img :src="staticData[0].char" alt="oop" class="h-60" />
                </div>

            </div>

        </div>

        <div id="last" class=" mt-4 mb-2">
            <div class="flex justify-between">
                <div class="flex">
                    <button class=" text-slate-600 hover:text-blue-700 font-bold ml-4 mr-2">Trading NFTs</button>
                    <button class=" text-slate-600 hover:text-blue-700 font-bold mx-2">Hot Auctions</button>
                    <button class=" text-slate-600 hover:text-blue-700 font-bold mx-2">Recent Bids</button>
                    <button class=" text-slate-600 hover:text-blue-700 font-bold mx-2">Best Creators</button>
                </div>

                <div class="flex">
                    <button class=" text-slate-600 hover:text-blue-700 font-bold mx-2 ">Arts</button>
                    <button class=" text-slate-600 hover:text-blue-700 font-bold mx-2">Music</button>
                    <button class=" text-slate-600 hover:text-blue-700 font-bold mx-2">Games</button>
                    <button class=" text-slate-600 hover:text-blue-700 font-bold mr-4 ml-2">Photography</button>
                </div>

            </div>
            <div class="border-r border-dashed border-b mb-4 w-full pt-2 "></div>

            <div id="last" class=" flex justify-between overflow-y-auto min-w-full mt-6 bg-gray-100  ">

                <div id="da1" class=" w-full bg-white rounded-xl   shadow ml-1 p-4">
                  <div class="absolute">
                    <h2 class=" bg-black bg-opacity-50 border-2 rounded-md mx-2 px-2 border-white border-opacity-50  ">0 0 0 0</h2>
                  </div>

                  <div>
                    <img :src="staticData[0].n3" alt="n3" class=" rounded-lg" />
                  </div>

                  <div class="flex justify-between">
                     <div>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">Timeless Ape Club</h3>
                                <p class="text-slate-400 font-medium mt-1 mr-4"><small> @AllanRuiz</small></p>
                     </div>

                     <div>
                      <p class="text-slate-400 font-medium mt-1 mr-4"><small> Current Bid</small></p>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">0.58 ETH</h3>

                     </div>
                  </div>

                </div>

                <div id="da2" class=" w-full bg-white rounded-xl   shadow ml-1 p-4">
                  <div class="absolute">
                    <h2 class=" bg-black bg-opacity-50 border-2 rounded-md mx-2 px-2 border-white border-opacity-50  ">0 0 0 0</h2>
                  </div>

                  <div>
                    <img :src="staticData[0].n4" alt="n4" class=" rounded-lg" />
                  </div>

                  <div class="flex justify-between">
                     <div>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">King Cat</h3>
                                <p class="text-slate-400 font-medium mt-1 mr-4"><small> @CarlJean</small></p>
                     </div>

                     <div>
                      <p class="text-slate-400 font-medium mt-1 mr-4"><small> Current Bid</small></p>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">0.64 ETH</h3>

                     </div>
                  </div>

                </div>

                <div id="da3" class=" w-full bg-white rounded-xl   shadow ml-1 p-4">
                  <div class="absolute">
                    <h2 class=" bg-black bg-opacity-50 border-2 rounded-md mx-2 px-2 border-white border-opacity-50  ">0 0 0 0</h2>
                  </div>

                  <div>
                    <img :src="staticData[0].n5" alt="n5" class=" rounded-lg" />
                  </div>

                  <div class="flex justify-between">
                     <div>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">Smoker Cat</h3>
                                <p class="text-slate-400 font-medium mt-1 mr-4"><small> @JackCroy</small></p>
                     </div>

                     <div>
                      <p class="text-slate-400 font-medium mt-1 mr-4"><small> Current Bid</small></p>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">0.34 ETH</h3>

                     </div>
                  </div>

                </div>

                <div id="da4" class=" w-full bg-white rounded-xl   shadow ml-1 p-4">
                  <div class="absolute">
                    <h2 class=" bg-black bg-opacity-50 border-2 rounded-md mx-2 px-2 border-white border-opacity-50  ">0 0 0 0</h2>
                  </div>

                  <div>
                    <img :src="staticData[0].n6" alt="n6" class=" rounded-lg" />
                  </div>

                  <div class="flex justify-between">
                     <div>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">Green Ape Club</h3>
                                <p class="text-slate-400 font-medium mt-1 mr-4"><small> @MiguelTaylor</small></p>
                     </div>

                     <div>
                      <p class="text-slate-400 font-medium mt-1 mr-4"><small> Current Bid</small></p>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">0.99 ETH</h3>

                     </div>
                  </div>

                </div>

                <div id="da5" class=" w-full bg-white rounded-xl   shadow ml-1 p-4">
                  <div class="absolute">
                    <h2 class=" bg-black bg-opacity-50 border-2 rounded-md mx-2 px-2 border-white border-opacity-50  ">0 0 0 0</h2>
                  </div>

                  <div>
                    <img :src="staticData[0].n7" alt="n7" class=" rounded-lg" />
                  </div>

                  <div class="flex justify-between">
                     <div>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">Angry Shark</h3>
                                <p class="text-slate-400 font-medium mt-1 mr-4"><small> @JamesWalker</small></p>
                     </div>

                     <div>
                      <p class="text-slate-400 font-medium mt-1 mr-4"><small> Current Bid</small></p>
                      <h3 class=" font-semibold text-lg mt-1 mr-6">0.84 ETH</h3>

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

export default {
    //   components:{LayoutView}
    data() {
        const staticData = [
      {
        bg: require('@/assets/widgets/bg-1.jpg'),
            mon: require('@/assets/widgets/nft-1.png'),
            boa: require('@/assets/widgets/boa.png'),
            char: require('@/assets/images/gol.png'),
            n3: require('@/assets/widgets/nft-3.png'),
            n4: require('@/assets/widgets/nft-4.png'),
            n5: require('@/assets/widgets/nft-5.png'),
            n6: require('@/assets/widgets/nft-6.png'),
            n7: require('@/assets/widgets/nft-7.png'),
      }
    ];
        return {
            staticData
        };
    }

};
</script>

<style >

      </style>
