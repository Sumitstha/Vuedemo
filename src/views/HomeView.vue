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

    <!-- starting of box -->
    <div class=" bg-gray-100 container mx-auto min-h-full relative">
        <div id="one" class="  flex  p-2 text-center">
            <div id="left" class=" rounded-lg w-1/4 h-full relative shadow  bg-white p-2 mb-8 mt-4 mr-4">
                <div id="lefttop" class=" ">
                    <div class=" text-2xl font-bold ">T-Wind Multi Application</div>
                    <div class=" text-xl font-semibold text-gray-400 font-mono p-1">We design and develop clean and high quality application</div>
                    <div class="p-2">
                        <button class="bg-blue-600 hover:bg-blue-700 px-4  rounded-lg text-white">Create New</button>
                    </div>
                </div>
                <div id="left bottom" class=" mt-8">
                    <img :src="require('@/assets/images/user.png')" alt="Image">
                </div>
            </div>

            <div id="right" class="  w-3/4 h-full   bg-slate-100 p-2 mr-4">

                <div id="top" class=" flex justify-between bg-gray-100 ">

                    <div id="div1" class=" rounded-md shadow h-20 w-48 pt-2  m-2 bg-white ">
                        <div class="flex justify-between relative">
                            <div><span><i class="fa-solid fa-user-group mt-5 ml-4  text-blue-500"></i></span></div>
                            <div>
                                <h3 class=" font-semibold text-2xl mt-1 mr-8">24k</h3>
                                <p class="text-slate-400 font-medium mr-4">Sessions</p>
                            </div>
                        </div>
                    </div>
                    <div id="div2" class="shadow rounded-md  h-20 w-48 pt-2 m-2 bg-white">
                        <div class="flex justify-between relative">
                            <div><span><i class="fa-regular fa-clock fa-xl mt-6 ml-4  text-blue-500"></i></span></div>
                            <div>
                                <h3 class=" font-semibold text-2xl mt-1 mr-8">01<span class="text-slate-400">m</span>03<span class="text-slate-400">s</span></h3>
                                <p class="text-slate-400 font-medium mr-4">Avg.Sessions</p>
                            </div>
                        </div>
                    </div>
                    <div id="div3" class=" shadow rounded-md h-20 w-48 pt-2 m-2 bg-white">
                        <div class="flex justify-between relative">
                            <div><span><i class="fa-solid fa-arrow-trend-up fa-xl mt-6 ml-4  text-blue-500"></i></span></div>
                            <div>
                                <h3 class=" font-semibold text-2xl mt-1 mr-8">$1800</h3>
                                <p class="text-slate-400 font-medium mr-4">Bounce Rate</p>
                            </div>
                        </div>
                    </div>
                    <div id="div4" class=" rounded-md shadow h-20 w-48 pt-2 m-2  bg-white">
                        <div class="flex justify-between relative">
                            <div><span><i class="fa-solid fa-rocket fa-lg mt-6 ml-4 text-blue-500"></i></span></div>
                            <div>
                                <h3 class=" font-semibold text-2xl mt-1 mr-8">75000</h3>
                                <p class="text-slate-400 font-medium mr-4">Goal Completions</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div>
                    <div id="bottom" class="bg-white rounded-md  shadow mt-4 h-80">

                        <canvas id="mychart" class=" m-6 pb-6 pl-6 pr-16 pt-6 min-w-full"></canvas>
                    </div>
                </div>

            </div>
        </div>

        <div id="two" class="flex justify-between bg-gray-100">

            <div id="d1" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Sessions Device</h1>
                    </div>
                    <hr />
                </div>
                <div>
                    <img :src="imageSrc" alt="My Image" />
                </div>

            </div>

            <div id="d2" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Live Visits Our New Site</h1>

                    </div>
                    <hr />
                </div>
                <div class="text-center">
                    <p class=" font-mono text-slate-400 uppercase m-4  font-medium text-sm">Right Now</p>
                    <h2 class=" font-mono text-slate-800 dark:text-slate-300  text-4xl font-bold leading-8 py-2">120</h2>
                    <div class="text-gray-600">Yesterday Visits:10,524<span><i class="fa-solid ml-2 text-blue-600 fa-caret-up"></i></span></div>
                    <img class=" mt-5 mb-5" :src="icam" alt="Mycam" />
                </div>
                <div class="text-center  m-6"> <button class="bg-blue-600 hover:bg-blue-700 px-4 py-1 rounded-lg text-white">More Details</button></div>
                <div>

                </div>
            </div>
            <div id="d3" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
                <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Activities</h1>
                    </div>
                    <hr />
                </div>
                <div><img class=" mt-5 mb-3" :src="ddd" alt="Mycamp" /></div>
              
            </div>

        </div>

        <div id="three" class="flex justify-between bg-gray-100">
          <div id="d1" class=" rounded-md shadow h-full w-full pt-2  m-2 bg-white ">
            <div>
                    <div class="card-header">
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Total Visits</h1>
                    </div>
                    <hr />
                    <div class="overflow-hidden" >
                      <div class="m-2 p-2">
<table class=" min-w-full">
  <thead class="bg-gray-100 ">
    <tr>
      <th class="p-3  text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">CHANNELS</th>
      <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">SESSIONS</th>
      <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">PREV.PERIOD</th>
      <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">% CHANGE</th>
    </tr>
  </thead>
  
  <tbody>
    <tr class="">
      <td class="p-3"><a href="#" class=" text-blue-500"> Organic Search</a></td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%<span class=" text-green-600"><i class=" ml-2 fa-solid fa-caret-up"></i></span></td>
    </tr>
    <tr class="">
      <td class="p-3"><a href="#" class=" text-blue-500"> Direct</a></td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%<span class=" text-red-600"><i class="fa-solid fa-caret-down"></i></span></td>
    </tr>
    <tr class="">
      <td class="p-3"><a href="#" class=" text-blue-500">Referral</a></td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%<span class=" text-red-600"><i class="fa-solid fa-caret-down"></i></span></td>
    </tr>
    <tr class="">
      <td class="p-3"><a href="#" class=" text-blue-500"> Email</a></td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%<span class=" text-green-600"><i class=" ml-2 fa-solid fa-caret-up"></i></span></td>
    </tr>
    <tr class="">
      <td class="p-3"><a href="#" class=" text-blue-500">Social</a></td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%<span class=" text-green-600"><i class=" ml-2 fa-solid fa-caret-up"></i></span></td>
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
                        <h1 class="font-mono text-xl ml-4 dark:text-slate-300 font-semibold">Browser used by users</h1>
                    </div>
                    <hr />
                    <div class="overflow-hidden" >
                      <div class="m-2 p-2">
<table class=" min-w-full">
  <thead class="bg-gray-100 ">
    <tr>
      <th class="p-3  text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">BROWSERS</th>
      <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">SESSIONS</th>
      <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">BOUNCE RATE</th>
      <th class="p-3 text-xs font-medium tracking-wider text-left text-gray-700 uppercase dark:text-gray-400">TRANSECTIONS</th>
    </tr>
  </thead>
  
  <tbody class="">
    <tr class="">
      <td class="p-3  text-sm font-mono font-semibold"><img class=" mr-2 h-6 inline-block" :src="chrome" alt="chr" />Chrome</td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%</td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
    </tr>
    <tr class="">
      <td class="p-3 text-sm font-mono font-semibold"><img class=" mr-2 h-6 inline-block" :src="explorer" alt="exp" />Explorer</td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%</td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
    </tr>
    <tr class="">
      <td class="p-3 text-sm font-mono font-semibold"><img class=" mr-2 h-6 inline-block" :src="safari" alt="saf" />Safari</td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%</td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
    </tr>
    <tr class="">
      <td class="p-3 text-sm font-mono font-semibold"><img class=" mr-2 h-6 inline-block" :src="mozilla" alt="moz" />Mozilla</td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%</td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
    </tr>
    <tr class="">
      <td class="p-3 text-sm font-mono font-semibold"><img class=" mr-2 h-6 inline-block" :src="opera" alt="opr" />Opera</td>
      <td class="p-3 font-mono text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">10853<small class="text-gray-400">(52%)</small></td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">52.80%</td>
      <td class="p-3 font-mono  text-sm text-gray-500 whitespace-nowrap dark:text-gray-400">566<small class="text-gray-400">(92%)</small></td>
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
// @ is an alias to /src
// import LayoutView from './LayoutView.vue';
import Chart from 'chart.js/auto';
export default {
    data() {
        return {
            name: 'HomeView',
            imageSrc: require('@/assets/images/sc.png'),
            icam: require('@/assets/images/camp.png'),
            chrome: require('@/assets/images/chrome.png'),
            explorer: require('@/assets/images/in-explorer.png'),
            safari: require('@/assets/images/safari.png'),
            mozilla: require('@/assets/images/mozilla.png'),
            opera: require('@/assets/images/opera.png'),
            ddd: require('@/assets/images/dd.png'),
        };
    },

    // components: {LayoutView}

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
        myChart;
    },

}
</script>
