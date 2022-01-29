<template>
<div class="flex flex-row  overflow-x-hidden">
    <div class="w-0 smlaptop:w-56 bg-white h-screen flex flex-col fixed sideBar">
        <div class="ml-2 h-9 mr-2 mt-2 cursor-pointer flex flex-col items-center p-1 w-0 smlaptop:w-52">
            <div class="bg-gray-200 ml-2 h-9 mr-2 cursor-pointer flex flex-row  rounded-md items-center p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm tracking-wider pl-1 text-hardBlue">Landing Page</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer flex flex-row items-center rounded-md p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm tracking-wider pl-1 text-hardBlue">Strand App</p>
            </div>
        </div>
        <div class="smlaptop:w-60 fixed bottom-1.5 flex justify-between px-3">
            <div class="font-sans w-4/5 bg-gray-200 py-2 px-2 w-32 text-xs h-8">
                New Project
            </div>
            <div class=" w-1/5 px-3">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M3 17V19H9V17H3ZM3 5V7H13V5H3ZM13 21V19H21V17H13V15H11V21H13ZM7 9V11H3V13H7V15H9V9H7ZM21 13V11H11V13H21ZM15 9H17V7H21V5H17V3H15V9Z" fill="#110F24" fill-opacity="0.4"/>
                </svg>
            </div>
        </div>
    </div>
    <div class="w-full mt-16 smlaptop:mt-2 px-3 smlaptop:px-0 pr-1 calcFn min-h-screen block h-14">
        <Head class="mt-2" />
        <div style="width: 99%;" class="rounded-md CustomMinimumH mt-6 smlaptop:mt-2 block relative my-2 chatBoxHeight bg-white">
            <div class="w-full rounded-t-xl h-14 flex flex-row items-center my-2 bg-gray-300 overflow-x-scroll smlaptop:overflow-x-hidden">
                <div style="border-bottom: 3px solid #575BDE;" class="h-full ml-3 flex items-center justify-center">
                    <p class="font-sans text-base font-medium">Overview</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Projects</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Invoices</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Estimates</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Expenses</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Edit</p>
                </div>
            </div>
            <div class="w-full pb-4 px-3 overflow-x-hidden flex flex-col border-b-2 border-gray-100">
                <div class="flex flex-col smlaptop:flex-row w-full">
                    <div class="w-full smlaptop:w-1/3 block p-2">
                        <p class="text-base text-gray-400">Amount Due</p>
                        <p class="text-2xl font-bold">$4000.00</p>
                    </div>
                    <div class="w-full smlaptop:w-1/3 block p-2">
                        <p class="text-base text-gray-400">Expenses</p>
                        <p class="text-2xl font-bold">$450.00</p>
                    </div>
                    <div class="w-full smlaptop:w-1/3 block p-2">
                        <p class="text-base text-gray-400">Latest invoice</p>
                        <p class="text-2xl font-bold">INV-20160827-3</p>
                    </div>
                </div>
            </div>
            <div class="w-full border-b-2 border-gray-100 flex justify-between py-4">
                <div class="flex flex-row">
                    <div class="lowOp">
                        <span class="material-icons px-3 pt-1">app_registration</span>
                    </div>
                    <div>
                        <p class="text-base pt-1">Giddify</p>
                        <p class="text-sm text-gray-400">Customer was created on June 17, 2018.</p>
                    </div>
                </div>
            </div>
            <div class="w-full border-b-2 border-gray-100 flex justify-between py-4">
                <div class="flex flex-row">
                    <div class="lowOp">
                        <span class="material-icons px-3 pt-1">person</span>
                    </div>
                    <div>
                        <p class="text-base pt-1">Mr. Rocco Erhart</p>
                        <p class="text-sm text-gray-400">rocco.erhart@example.com</p>
                    </div>
                </div>
            </div>
            <div class="w-full border-b-2 border-gray-100 flex flex-col py-4">
                <div class="flex flex-row">
                    <div class="lowOp">
                        <span class="material-icons px-3 pt-1">message</span>
                    </div>
                    <div>
                        <p class="text-base pt-1">Information</p>
                        <p class="text-sm text-gray-400">Address and details.</p>
                    </div>
                </div>
                <div class="flex flex-col smlaptop:flex-row w-full ml-12 mt-3">
                    <div class="w-4/5 bg-gray-300 smlaptop:w-2/5">
                        <div class="block p-3">
                            <p>7th Street Northeast</p>
                            <p>Atlanta</p>
                            <p>GA-30309</p>
                            <p>USA</p>
                        </div>
                    </div>
                    <div class="w-4/5 bg-gray-300 smlaptop:w-2/5 smlaptop:ml-8 mt-3">
                        <div class="block p-3">
                            <p>Currency: USD</p>
                            <p>Website: example.com</p>
                            <p>Portal: Disabled</p>
                            <p>Language: English</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="w-full flex justify-start flex-col py-4">
                <div class="flex flex-row">
                    <div class="lowOp">
                        <span class="material-icons px-3 pt-1">credit_card</span>
                    </div>
                    <div>
                        <p class="text-base pt-1">Payments</p>
                        <p class="text-sm text-gray-400">$16.600 in total for the past 6 months</p>
                    </div>
                </div>
                <div class="pt-8 overflow-x-hidden relative flex flex-row items-end smlaptop:ml-8">
                    <div class="w-full mb-6 absolute flex flex-col">
                        <div class="h-1 border border-t-0 border-l-0 border-r-0 border-gray-200 mt-9"></div>
                        <div class="h-1 border border-t-0 border-l-0 border-r-0 border-gray-200 mt-9"></div>
                        <div class="h-1 border border-t-0 border-l-0 border-r-0 border-gray-200 mt-9"></div>
                        <div class="h-1 border border-t-0 border-l-0 border-r-0 border-gray-200 mt-9"></div>
                    </div>
                    <div v-for="(graph, i) in graphs" :key="i" :class="{'pl-2': i!=0, 'pr-2': i===graphs.length-1}" class="flex has-tooltip w-14 smlaptop:w-1/6 flex-col z-0">
                        <div class='tooltip text-center text-xs rounded mb-2 text-white bg-hoverBlue py-2'>{{ graph.status }}</div>
                        <div :class="graphHeight(i)" class="bg-blueish rounded h-10 cursor-pointer" />
                        <p class="text-center font-sans text-gray-400">{{ graph.month }}</p>
                    </div>
                </div>
            </div>
            <div class="w-full flex justify-start py-4">
                <div class="flex flex-row">
                    <div class="lowOp">
                        <span class="material-icons px-3 pt-1">file_copy</span>
                    </div>
                    <div>
                        <p class="text-base pt-1">Files</p>
                        <p class="text-sm text-gray-400">3 files have been favorited.</p>
                        <p class="text-base ">agreement.zip</p>
                        <p class="text-base ">license.zip</p>
                        <p class="text-base ">portal.zip</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="h-12 w-full" />
    </div>
</div>
</template>

<script>
import 'material-icons/iconfont/material-icons.css';
import Head from '~/components/Head'
export default {
  components: {
    Head
  },
  data () {
    return {
      graphs: [
        {
          month: 'Jul',
          status: '65'
        },
        {
          month: 'Aug',
          status: '85'
        },
        {
          month: 'Sept',
          status: '29'
        },
        {
          month: 'Oct',
          status: '62'
        },
        {
          month: 'Nov',
          status: '35'
        },
        {
          month: 'Dec',
          status: '45'
        }
      ]
    }
  },
  methods: {
    graphHeight (id) {
      const status = parseInt(this.graphs[id].status) 
      if (status > 80) {
        return 'h-24'
      } else if (status > 60 && status < 80) {
        return 'h16'
      } else if (status > 40 && status < 60) {
        return 'h-12'
      } else if (status > 20 && status < 40) {
        return 'h-8'
      }
    }
  }
}
</script>

<style>

@media screen and (min-width: 580px) {
  .sideBar {
    left: 15rem;
  }
    .calcFn {
        width: calc(100% - 15rem);
        margin-left: auto;
    }
}
.lowOp {
    opacity: 0.5;
}
.hoverSec:hover {
    border-bottom: 3px solid #929294;
}
.chip {
  display: inline-block;
  padding: 0 15px;
  height: 50px;
  font-size: 18px;
  line-height: 50px;
  border-radius: 25px;
  background-color: #f1f1f1;
}
</style>