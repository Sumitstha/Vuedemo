<template>
<body class="font-[Poppins] bg-gradient-to-t from-slate-50 to-slate-200   h-auto">
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
                                <li class="text-blue-500 hover:text-blue-600 px-1">Analytics</li>
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
    </div>

    <!-- starting of body -->

    <div class=" bg-gray-100 container mx-auto min-h-full relative">
        <div id="one " class=" flex justify-between bg-gray-100">
            <div id="ek" class="rounded-lg w-2/3 h-full relative shadow  bg-white p-2 ml-4 mr-4">
                <div id="top" class="flex justify-between  bg-gray-100">
                    <div class="border-r border-dashed dark:border-slate-700 border-b h-20 w-full pt-2  bg-white">
                        <div class=" text-center">
                            <h1 class="font-mono text-xl  dark:text-slate-300 font-semibold">520</h1>
                            <P class="text-slate-400">TODAY'S ORDER</P>
                        </div>
                    </div>
                    <div class="border-r border-dashed dark:border-slate-700 border-b h-20 w-full pt-2   bg-white">
                        <div class=" text-center">
                            <h1 class="font-mono text-xl  dark:text-slate-300 font-semibold">82.8</h1>
                            <P class="text-slate-400">CONVERSION RATE</P>
                        </div>
                    </div>
                    <div class="border-r border-dashed dark:border-slate-700 border-b h-20 w-full pt-2   bg-white">
                        <div class=" text-center">
                            <h1 class="font-mono text-xl  dark:text-slate-300 font-semibold">$92.5</h1>
                            <P class="text-slate-400">AVG.VALUE</P>
                        </div>
                    </div>
                    <div class="border-r border-dashed dark:border-slate-700 border-b h-20 w-full pt-2   bg-white">
                        <div class="text-center">
                            <h1 class="font-mono text-xl  dark:text-slate-300 font-semibold">$360.50</h1>
                            <P class="text-slate-400">GROSS SALE</P>
                        </div>
                    </div>
                </div>
                <div id="bottom" class="relative overflow h-81">
                    <div class="font-medium py-2 px-4  dark:text-slate-300">
                        <h4>Revenue Status</h4>
                    </div>
                    <div class="h-90">
                        <canvas id="mychart" class=" pl-6 pr-6 relative "></canvas>
                    </div>
                </div>
            </div>
            <div id="dui" class="rounded-lg w-1/3 h-full relative  bg-slate-100  mr-4">
                <div id="topp" class="flex justify-between rounded-lg shadow bg-gray-100">

                    <div class=" rounded-s-lg h-20 w-full pt-6 text-center bg-white">
                        barchart
                    </div>
                    <div class=" h-20 w-full pt-5  bg-white">
                        <div class="text-center">
                            <h1 class="font-mono text-xl  dark:text-slate-300 font-semibold">$25,200</h1>
                            <small class="text-slate-400">TODAY'S REVENUE</small>
                        </div>
                    </div>
                    <div class="rounded-e-lg h-20 w-full pt-6  bg-white">
                        <i class="fa-solid fa-download absolute ml-4 mt-2 text-white"></i>
                        <button class="bg-blue-600 hover:bg-blue-700 px-8 py-1 pr-4 rounded-lg text-white"> Withdraw</button>
                    </div>

                </div>
                <div id="bott" class="rounded-lg w-full h-full relative shadow  bg-white mt-2 p-2 mr-4">
                    <div class="pt-4 pb-6">
                        <img class="h-78 w-70 mt-5 mb-5" :src="map" alt="mapp" />
                    </div>
                    <div class=" flex justify-between pb-8 pt-2 bg-white">
                        <div class="border-r border-dashed  border-b  w-full pt-2  bg-white">
                            <div class=" text-center">
                                <h1 class="font-mono text-xl  dark:text-slate-300 font-semibold">$15,520
                                    <span class="w-1 h-1 rounded-full bg-pink-500 relative inline-block self-center mb-4 "></span>

                                </h1>
                                <P class="text-slate-400"><small>DOMESTIC</small>
                                </P>
                            </div>
                        </div>
                        <div class="border-r border-dashed  border-b  w-full pt-2  bg-white">
                            <div class=" text-center">
                                <h1 class="font-mono text-xl  dark:text-slate-300 font-semibold">$36,880
                                    <span class="w-1 h-1 rounded-full bg-blue-500 relative inline-block self-center mb-4 "></span>
                                </h1>
                                <P class="text-slate-400"><small>INTERNATIONAL</small></P>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div id="two" class="flex justify-between mx-2 bg-gray-100">

            <div id="d1" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Order By Device</h1>
                    </div>
                    <hr />
                </div>
                <div>
                    <img :src="cha" alt="oo" />
                </div>

            </div>

            <div id="d2" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Reports Overview</h1>

                    </div>
                    <hr />
                </div>
                <div id="sec">
                    <div id="sec1" class="mb-2">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">$8836.68</h1>
                    </div>
                    <div id="sec2" class="w-full px-4 mb-2">
                        <div class="flex items-center">
                            <div class="w-1/4 bg-blue-500 h-2 rounded-tl rounded-bl mr-0.5">

                            </div>
                            <div class="w-1/4 bg-yellow-500 h-2  mr-0.5">

                            </div>
                            <div class="w-1/4 bg-gray-500 h-2  mr-0.5">
                                <div class=" h-2 w-1/2 bg-pink-500">

                                </div>

                            </div>
                            <div class="w-1/4 bg-gray-500 h-2 rounded-tr rounded-br mr-0.5">

                            </div>
                        </div>

                    </div>
                    <div class="overflow-hidden">
                        <div class="m-2 p-2">
                            <table class=" min-w-full">
                                <thead class="bg-gray-100 ">
                                    <tr>
                                        <th class="p-3  text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">DEVICE</th>
                                        <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">AMOUNT</th>

                                        <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">% CHANGE</th>
                                    </tr>
                                </thead>

                                <tbody>
                                    <tr class="border-b border-dashed">
                                        <td class="p-3">
                                            <span class="w-1 h-1 rounded-full bg-blue-500 relative inline-block self-center mr-2"></span>
                                            Gross value</td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">$6,543.55</td>
                                        <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">
                                            <span class=" bg-green-400 rounded-sm p-1 ">+6.8</span></td>

                                    </tr>
                                    <tr class="border-b border-dashed">
                                        <td class="p-3">
                                            <span class="w-1 h-1 rounded-full bg-yellow-500 relative inline-block self-center mr-2"></span>
                                            Net volume from sales</td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">$3,654.21</td>
                                        <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">
                                            <span class=" bg-blue-400 rounded-sm p-1 ">+4.5</span></td>

                                    </tr>
                                    <tr class="">
                                        <td class="p-3">
                                            <span class="w-1 h-1 rounded-full bg-pink-500 relative inline-block self-center mr-2"></span>
                                            Other</td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">$563.20</td>
                                        <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">
                                            <span class=" bg-pink-400 rounded-sm p-1 ">-1.2</span></td>

                                    </tr>

                                </tbody>
                            </table>
                        </div>
                    </div>
                </div>

            </div>
            <div id="d3" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Top Dealer</h1>
                    </div>
                    <hr />
                </div>
                <div id="top dealer ko tala ko div" class="block">
                    <div class=" flex justify-start">
                        <div>
                            <img class="h-14 w-14  p-2 ml-4" :src="franky" alt="fra" />
                        </div>
                        <div>
                            <h1 class="font-mono text-md  dark:text-slate-300 font-semibold">Fitbit Incorporation</h1>
                            <small class="text-slate-400">San Diego, California</small>
                        </div>

                    </div>
                    <div class=" flex justify-between pb-8 pt-2 bg-white">
                        <div class="border-r border-dashed    w-full pt-2  bg-white">
                            <div class=" text-center">
                                <h1 class="font-mono text-xl  dark:text-slate-300 font-semibold">5520

                                </h1>
                                <p class="text-slate-400"><small>PRODUCTS SOLD</small>
                                </p>
                            </div>
                        </div>
                        <div class="border-r border-dashed    w-full pt-2  bg-white">
                            <div class=" text-center">
                                <h1 class="font-mono text-xl  dark:text-slate-300 font-semibold">$36,880

                                </h1>
                                <p class="text-slate-400"><small>TOTAL EARNING</small></p>
                            </div>
                        </div>
                    </div>

                    <div class="flex justify-end mr-2">
                        <p class="text-slate-400"><small>73%</small></p>

                    </div>

                    <div class=" flex items-center p-2 mb-4">
                        <div class="w-full relative bg-gray-500 h-2 rounded-full mx-5">
                            <div class="h-2 w-2/3  bg-blue-500 rounded-full"></div>
                        </div>

                    </div>

                    <div class=" flex justify-center px-6 mb-4">
                        <button class="bg-blue-600 w-full hover:bg-blue-700 px-4 py-1 rounded-lg text-white">Send Message</button>
                    </div>
                </div>

            </div>

        </div>
        <div id="three" class="flex justify-between bg-gray-100 mx-2">
            <div id="d1" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Earning Reports </h1>
                    </div>
                    <hr />
                    <div class="overflow-hidden">
                        <div class="m-2 p-2">
                            <table class=" min-w-full">
                                <thead class="bg-gray-100 ">
                                    <tr>
                                        <th class="p-3  text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">DATE</th>
                                        <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">ITEM COUNTS</th>
                                        <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">TAX</th>
                                        <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">EARNING</th>
                                    </tr>
                                </thead>

                                <tbody>
                                    <tr class="">
                                        <td class="p-3"><a href="#" class=" text-gray-500"> 03 March</a></td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">50</td>
                                        <td class="p-3 font-mono  text-sm  whitespace-nowrap dark:text-gray-400 text-red-600">$-40</td>
                                        <td class="p-3 font-mono  text-sm text-gray-900 font-bold whitespace-nowrap dark:text-gray-400">$15,500.00</td>
                                        
                                    </tr>
                                    <tr class="">
                                        <td class="p-3"><a href="#" class=" text-gray-500"> 04 March</a></td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">120</td>
                                        <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">-</td>
                                        <td class="p-3 font-mono  text-sm text-gray-900 font-bold whitespace-nowrap dark:text-gray-400">$20,900.00</td>
                                    </tr>
                                    <tr class="">
                                        <td class="p-3"><a href="#" class=" text-gray-500">05 March</a></td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">90</td>
                                        <td class="p-3 font-mono  text-sm text-red-600 whitespace-nowrap dark:text-gray-400">$-20</td>
                                        <td class="p-3 font-mono  text-sm text-gray-900 font-bold whitespace-nowrap dark:text-gray-400"> $10,500.00</td>
                                    </tr>
                                    <tr class="">
                                        <td class="p-3"><a href="#" class=" text-gray-500"> 06 March</a></td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">160</td>
                                        <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">-</td>
                                        <td class="p-3 font-mono  text-sm text-gray-900 font-bold whitespace-nowrap dark:text-gray-400">$35,000.00</td>
                                    </tr>
                                    <tr class="">
                                        <td class="p-3"><a href="#" class=" text-gray-500">07 March</a></td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">80</td>
                                        <td class="p-3 font-mono  text-sm  text-red-600 whitespace-nowrap dark:text-gray-400">$-60</td>
                                        <td class="p-3 font-mono  text-sm text-gray-900 font-bold whitespace-nowrap dark:text-gray-400">$18,880.00</td>
                                    </tr>

                                </tbody>
                            </table>
                        </div>
                    </div>

                </div>
            </div>

            <div id="d2" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Most Popular Products </h1>
                    </div>
                    <hr />
                    <div class="overflow-hidden">
                        <div class="m-2 p-2 mb-10">
                            <table class=" min-w-full mb-4">
                                <thead class="bg-gray-100  mb-2">
                                    <tr>
                                        <th class="p-3  text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">PRODUCT</th>
                                        <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">PRICE</th>
                                        <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">SALE</th>
                                        <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">STATUS</th>
                                        <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">ACTION</th>
                                    </tr>
                                </thead>

                                <tbody class=" ">
                                    <tr class=" ">
                                        <td class="p-3   text-sm font-mono font-semibold"><img class=" mr-2 h-6 inline-block" :src="cam" alt="cam" />T-Wind Camera EDM 5D(White)</td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">$50 <del class="text-gray-400">$90</del></td>
                                        <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">450<small class="text-gray-400">(500)</small></td>
                                        <td><span class=" bg-green-200 text-green-900 rounded-sm p-1 ">Stock</span></td>
                                        <td><span><i class="fa-regular fa-pen-to-square text-gray-600 ml-6"></i></span> <span><i class="fa-regular fa-trash-can text-red-600"></i></span></td>
                                    </tr>
                                    <tr class="">
                                        <td class="p-3 text-sm font-mono font-semibold"><img class=" mr-2 h-6 inline-block" :src="shoe" alt="shoes" />T-Wind Shoes Max-Zon</td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">$49 <del class="text-gray-400">$88</del></td>
                                        <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">850<small class="text-gray-400">(900)</small></td>
                                        <td><span class=" bg-green-200 text-green-900 rounded-sm p-1 ">Stock</span></td>
                                        <td><span><i class="fa-regular fa-pen-to-square text-gray-600 ml-6"></i></span> <span><i class="fa-regular fa-trash-can text-red-600"></i></span></td>
                                    </tr>
                                    <tr class="">
                                        <td class="p-3 text-sm font-mono font-semibold"><img class=" mr-2 h-6 inline-block" :src="vr" alt="vr" />T-Wind VR 5D (Black)</td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">$39 <del class="text-gray-400">$99</del></td>
                                        <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">700<small class="text-gray-400">(700)</small></td>
                                        <td><span class=" bg-red-200 text-red-900 rounded-sm p-1 ">Sold</span></td>
                                        <td><span><i class="fa-regular fa-pen-to-square text-gray-600 ml-6"></i></span> <span><i class="fa-regular fa-trash-can text-red-600"></i></span></td>
                                    </tr>
                                    <tr class="">
                                        <td class="p-3 text-sm font-mono font-semibold"><img class=" mr-2 h-6 inline-block" :src="mask" alt="mask" />T-Wind Mask N99 [ISI]</td>
                                        <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">$5 <del class="text-gray-400">$9</del></td>
                                        <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">1850<small class="text-gray-400">(2000)</small></td>
                                        <td><span class=" bg-green-200 text-green-900 rounded-sm p-1 ">Stock</span></td>
                                        <td><span><i class="fa-regular fa-pen-to-square text-gray-600 ml-6"></i></span> <span><i class="fa-regular fa-trash-can text-red-600"></i></span></td>
                                    </tr>
                                   

                                </tbody>
                            </table>
                        </div>
                    </div>

                </div>

            </div>
        </div>
    </div>

</body>
</template>

<script>
// import LayoutView from './LayoutView.vue';
import Chart from 'chart.js/auto';
export default {
    // components:{LayoutView}
    data() {
        return {
            map: require('@/assets/images/map.png'),
            cha: require('@/assets/images/oo.png'),
            franky: require('@/assets/images/avatar-8.jpg'),
            cam: require('@/assets/images/01.png'),
            shoe: require('@/assets/images/02.png'),
            vr: require('@/assets/images/03.png'),
            mask: require('@/assets/images/04.png'),
        }
    },
    mounted() {
        console.log('component mounted.')
        const ctx = document.getElementById('mychart');
        const myChart = new Chart(ctx, {
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
        myChart;
    },

}
</script>

<style >

         </style>
