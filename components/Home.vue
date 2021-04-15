<template>
<div>
  <div class="w-full fixed smlaptop:hidden z-10 bg-DarkBlue p-4 flex justify-between items-center">
    <div class="flex content-center">
      <div class="flex-initial">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <g id="Icon">
          <path id="Icon_2" fill-rule="evenodd" clip-rule="evenodd" d="M24 12C24 18.6274 18.6274 24 12 24C5.37258 24 0 18.6274 0 12C0 5.37258 5.37258 0 12 0C18.6274 0 24 5.37258 24 12ZM10.6078 5.31363L9.05221 5.03418H9.05158C8.47404 4.9305 7.87974 5.06484 7.39938 5.40765C6.91902 5.75046 6.59195 6.27366 6.49009 6.8622L5.00968 15.4228C4.98047 15.5909 5.01797 15.7639 5.11395 15.9039C5.20992 16.0438 5.35651 16.1392 5.52148 16.169L8.01094 16.6159C8.34097 16.6752 8.68062 16.5985 8.95517 16.4027C9.22971 16.2068 9.41667 15.9078 9.47491 15.5715L11.1202 6.0599C11.1347 5.97661 11.1329 5.89124 11.115 5.80865C11.097 5.72606 11.0633 5.64788 11.0157 5.57858C10.9682 5.50928 10.9076 5.45021 10.8376 5.40475C10.7676 5.35929 10.6895 5.32833 10.6078 5.31363ZM18.4774 8.03601L13.4998 7.141C13.3363 7.11163 13.1688 7.11537 13.0067 7.15199C12.8447 7.18862 12.6913 7.25742 12.5553 7.35447C12.4194 7.45151 12.3035 7.5749 12.2144 7.71758C12.1252 7.86027 12.0645 8.01945 12.0358 8.18604L10.3898 17.697C10.3753 17.7804 10.377 17.8659 10.3949 17.9486C10.4129 18.0313 10.4466 18.1095 10.4943 18.1789C10.5419 18.2483 10.6026 18.3074 10.6727 18.3529C10.7428 18.3984 10.821 18.4293 10.9029 18.4439L13.7026 18.9461C14.152 19.0269 14.6127 19.0167 15.0582 18.9161C15.5038 18.8155 15.9255 18.6264 16.2994 18.3597C16.6733 18.093 16.9919 17.7538 17.2371 17.3616C17.4824 16.9694 17.6494 16.5317 17.7287 16.0737L18.9905 8.78164C19.0048 8.69835 19.0029 8.61299 18.9849 8.53045C18.9669 8.4479 18.9331 8.36977 18.8855 8.30053C18.8378 8.23129 18.7773 8.17229 18.7073 8.12691C18.6372 8.08152 18.5591 8.05063 18.4774 8.03601Z" fill="white"/>
          </g>
        </svg>
      </div>
      <div class="flex-initial pl-3">
        <p class="font-sans text-sm cursor-pointer text-white font-black">Dashboard UI Kit 2.0</p>
      </div>
    </div>
    <div class="burger cursor-pointer">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path fill-rule="evenodd" clip-rule="evenodd" d="M3 18H21V16H3V18ZM3 13H21V11H3V13ZM3 6V8H21V6H3Z" fill="white"/>
      </svg>
    </div>
  </div>
  <div class="w-auto pt-3 px-2 flex items-center justify-between h-14">
    <div class="flex h-8 rounded justify-start bg-white items-center">
      <div class="pl-2">
        <svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M11.625 10.5H11.0325L10.8225 10.2975C11.5575 9.4425 12 8.3325 12 7.125C12 4.4325 9.8175 2.25 7.125 2.25C4.4325 2.25 2.25 4.4325 2.25 7.125C2.25 9.8175 4.4325 12 7.125 12C8.3325 12 9.4425 11.5575 10.2975 10.8225L10.5 11.0325V11.625L14.25 15.3675L15.3675 14.25L11.625 10.5ZM7.125 10.5C5.2575 10.5 3.75 8.9925 3.75 7.125C3.75 5.2575 5.2575 3.75 7.125 3.75C8.9925 3.75 10.5 5.2575 10.5 7.125C10.5 8.9925 8.9925 10.5 7.125 10.5Z" fill="#110F24" fill-opacity="0.4"/>
        </svg>
      </div>
      <div>
        <input type="text" class="focus:outline-none pl-2" placeholder="Search...">
      </div>
    </div>
    <div class="flex flex-row">
      <div class="book cursor-pointer">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M13 12H20V13.5H13V12ZM13 9.5H20V11H13V9.5ZM13 14.5H20V16H13V14.5ZM21 4H3C1.9 4 1 4.9 1 6V19C1 20.1 1.9 21 3 21H21C22.1 21 23 20.1 23 19V6C23 4.9 22.1 4 21 4ZM21 19H12V6H21V19Z" fill="#110F24" fill-opacity="0.4"/>
        </svg>
      </div>
      <div class="bell cursor-pointer pl-2">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M12 22C13.1 22 14 21.1 14 20H10C10 21.1 10.89 22 12 22ZM18 16V11C18 7.93 16.36 5.36 13.5 4.68V4C13.5 3.17 12.83 2.5 12 2.5C11.17 2.5 10.5 3.17 10.5 4V4.68C7.63 5.36 6 7.92 6 11V16L4 18V19H20V18L18 16Z" fill="#110F24" fill-opacity="0.4"/>
        </svg>
      </div>
    </div>
  </div>
  <div class="rounded-xl m-2 h-64 bg-white">
    <div class="w-full rounded-t-xl h-14 flex justify-between items-center my-2 bg-gray-300">
      <p class="pl-3 font-sans text-base font-bold">This Month</p>
      <select @click="randomizeTheGraph()" name="cars" class="mr-3 focus:outline-none cursor-pointer bg-white w-28 border border-gray-200" id="cars">
        <option value="volvo">Sales</option>
        <option value="volvo">Stock</option>
      </select>
    </div>
    <div class="pt-8 overflow-x-hidden relative flex flex-row items-end">
      <div class="w-full mb-6 absolute flex flex-col">
        <div class="h-1 border border-t-0 border-l-0 border-r-0 border-gray-200 mt-9"></div>
        <div class="h-1 border border-t-0 border-l-0 border-r-0 border-gray-200 mt-9"></div>
        <div class="h-1 border border-t-0 border-l-0 border-r-0 border-gray-200 mt-9"></div>
        <div class="h-1 border border-t-0 border-l-0 border-r-0 border-gray-200 mt-9"></div>
      </div>
      <div v-for="(graph, i) in graphs" :key="i" class="flex has-tooltip w-14 smlaptop:w-1/12 flex-col pl-2 z-0">
        <div class='tooltip text-center rounded mb-2 text-white bg-hoverBlue'>{{ graph.status }}</div>
        <div :class="graphHeight(i)" class="bg-blueish rounded h-10 cursor-pointer" />
        <p class="text-center font-sans text-gray-400">{{ graph.month }}</p>
      </div>
    </div>
  </div>
  <div class="flex smlaptop:justify-between flex-wrap smlaptop:flex-nowrap">
    <div class="rounded-xl m-2 w-full smlaptop:w-3/5 bg-white">
      <div class="w-full rounded-t-xl h-14 flex justify-between items-center bg-gray-300">
        <p class="pl-3 text-base font-bold font-sans">Tasks</p>
        <div class="w-3/5 tablet:w-1/5 flex flex-row justify-end">
          <select name="cars" class="mr-3 text-base focus:outline-none bg-white w-28 border border-gray-200" id="cars">
            <option value="volvo">Sort By</option>
          </select>
          <div class="mr-4 bg-gray-200 p-2">
            <svg width="10" height="10" viewBox="0 0 10 10" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path fill-rule="evenodd" clip-rule="evenodd" d="M5.00004 0.333344C4.63185 0.333344 4.33337 0.63182 4.33337 1.00001V4.33334H1.00004C0.631851 4.33334 0.333374 4.63182 0.333374 5.00001C0.333374 5.3682 0.631851 5.66668 1.00004 5.66668H4.33337V9.00001C4.33337 9.3682 4.63185 9.66668 5.00004 9.66668C5.36823 9.66668 5.66671 9.3682 5.66671 9.00001V5.66668H9.00004C9.36823 5.66668 9.66671 5.3682 9.66671 5.00001C9.66671 4.63182 9.36823 4.33334 9.00004 4.33334H5.66671V1.00001C5.66671 0.63182 5.36823 0.333344 5.00004 0.333344Z" fill="#110F24"/>
            </svg>
          </div>
        </div>
      </div>
      <div v-for="(task, i) in toDoList" :key="i" class="flex flex-row h-14 items-center px-3 border-gray-200 border border-t-0 border-l-0 border-r-0">
        <div class="flex justify-center w-1/12">
          <input type="checkbox" v-model="task.checked" class="checked:bg-gray-200 checked:border-red">
        </div>
        <div @click="toDoList[i].checked = !toDoList[i].checked" class="w-7/12 flex justify-start cursor-pointer">
          <strike class="font-sans text-gray-400 text-base" v-if="task.checked">{{ task.taskName }}</strike>
          <p class="font-sans text-base" v-else>{{ task.taskName }}</p>
        </div>
        <div class="w-2/12 text-sm text-gray-400">{{ task.due }}</div>
        <div class="w-1/12 flex justify-end">
          <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M11 3.99999V11.6667C11 13.14 9.80669 14.3333 8.33335 14.3333C6.86002 14.3333 5.66669 13.14 5.66669 11.6667V3.33332C5.66669 2.41332 6.41335 1.66666 7.33335 1.66666C8.25335 1.66666 9.00002 2.41332 9.00002 3.33332V10.3333C9.00002 10.7 8.70002 11 8.33335 11C7.96669 11 7.66669 10.7 7.66669 10.3333V3.99999H6.66669V10.3333C6.66669 11.2533 7.41335 12 8.33335 12C9.25335 12 10 11.2533 10 10.3333V3.33332C10 1.85999 8.80669 0.666656 7.33335 0.666656C5.86002 0.666656 4.66669 1.85999 4.66669 3.33332V11.6667C4.66669 13.6933 6.30669 15.3333 8.33335 15.3333C10.36 15.3333 12 13.6933 12 11.6667V3.99999H11Z" fill="#110F24" fill-opacity="0.4"/>
          </svg>
        </div>
        <div @click="toDoList[i].bookmark = !toDoList[i].bookmark" v-if="task.bookmark" class="w-1/12 flex justify-end cursor-pointer">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M21.3333 0H2.66667C1.18667 0 0 1.2 0 2.66667V21.3333C0 22.8 1.18667 24 2.66667 24H21.3333C22.8133 24 24 22.8 24 21.3333V2.66667C24 1.2 22.8133 0 21.3333 0ZM12 16.216L16.944 19.2L15.632 13.576L20 9.792L14.248 9.304L12 4L9.752 9.304L4 9.792L8.368 13.576L7.056 19.2L12 16.216Z" fill="#575BDE"/>
          </svg>
        </div>
        <div @click="toDoList[i].bookmark = !toDoList[i].bookmark" v-else class="w-1/12 flex justify-end cursor-pointer">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M21.3333 0H2.66667C1.18667 0 0 1.2 0 2.66667V21.3333C0 22.8 1.18667 24 2.66667 24H21.3333C22.8133 24 24 22.8 24 21.3333V2.66667C24 1.2 22.8133 0 21.3333 0ZM12 16.216L16.944 19.2L15.632 13.576L20 9.792L14.248 9.304L12 4L9.752 9.304L4 9.792L8.368 13.576L7.056 19.2L12 16.216Z" fill="#ECECEE"/>
          </svg>
        </div>
      </div>
    </div>
    <div class="rounded-xl m-2 w-full smlaptop:w-2/5 bg-white">
      <div class="w-full rounded-t-xl h-14 flex justify-between items-center bg-gray-300">
        <p class="pl-3 font-sans text-base font-bold">Projects</p>
        <div class="mr-4 bg-gray-200 p-2">
          <svg width="10" height="10" viewBox="0 0 10 10" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M5.00004 0.333344C4.63185 0.333344 4.33337 0.63182 4.33337 1.00001V4.33334H1.00004C0.631851 4.33334 0.333374 4.63182 0.333374 5.00001C0.333374 5.3682 0.631851 5.66668 1.00004 5.66668H4.33337V9.00001C4.33337 9.3682 4.63185 9.66668 5.00004 9.66668C5.36823 9.66668 5.66671 9.3682 5.66671 9.00001V5.66668H9.00004C9.36823 5.66668 9.66671 5.3682 9.66671 5.00001C9.66671 4.63182 9.36823 4.33334 9.00004 4.33334H5.66671V1.00001C5.66671 0.63182 5.36823 0.333344 5.00004 0.333344Z" fill="#110F24"/>
          </svg>
        </div>
      </div>
      <div v-for="(project, i) in projects" :key="i" class="flex flex-row h-14 items-center px-3 border-gray-200 border border-t-0 border-l-0 border-r-0">
        <div class="w-6/12 flex flex-col">
          <div class="font-sans text-base">{{ project.name }}</div>
          <div class="font-sans text-xs text-gray-400">{{ project.sub }}</div>
        </div>
        <div class="w-6/12 h-1 bg-gray-300">
          <div :class="progressBar(i)" class="h-1"></div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>
<script>
export default {
  data () {
    return {
      toDoList: [
        {
          taskName: 'Send prototype to team',
          due: 'Today',
          bookmark: false,
          checked: false
        },
        {
          taskName: 'Review content with copywriter',
          due: 'Today',
          bookmark: false,
          checked: false
        },
        {
          taskName: 'Optimize hero images',
          due: 'Today',
          bookmark: false,
          checked: false
        },
        {
          taskName: 'Add loading screen after sign up',
          due: 'Today',
          bookmark: false,
          checked: true
        },
        {
          taskName: 'Get file structure ready for cms',
          due: '13 April',
          bookmark: true,
          checked: false
        },
      ],
      graphs: [
        {
          month: 'Jan',
          status: '45'
        },
        {
          month: 'Feb',
          status: '65'
        },
        {
          month: 'Mar',
          status: '15'
        },
        {
          month: 'Apr',
          status: '25'
        },
        {
          month: 'May',
          status: '75'
        },
        {
          month: 'Jun',
          status: '95'
        },
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
      ],
      projects: [
        {
          name: 'Flowychart Editor',
          sub: 'Enigm',
          status: '45%'
        },
        {
          name: 'ProjectX',
          sub: 'Giddify',
          status: '85%'
        },
        {
          name: 'Landing Page',
          sub: 'Mondemi',
          status: '25%'
        }
      ],
      tasks: [
        {
          name: 'enigma',
          status: false,
          due: 'Today'
        }
      ]
    }
  },
  methods () {
    const device = navigator.userAgent.toLowerCase()
    const isAndroid = device.includes('android')
    if (isAndroid || !!navigator.platform && /iPad|iPhone|iPod/.test(navigator.platform)) {
      this.graphs = this.graphs.slice(5, 12)
      this.isMobileDevice = true
    } else {
      console.log('big screen device')
    }
    this.previewChat = {...this.ChatJson[0]}
  },
  methods: {
    randomizeTheGraph () { // onchanging the dropdown random number will be generated graph will change
      this.graphs.map((key) => {
        const randomNum = Math.floor(Math.random() * (76)) + 25 // random num b/w 25 and 100
        key.status = randomNum
      })
    },
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
    },
    progressBar (id) {
      const status = parseInt(this.projects[id].status.substring(0, 2))
      if (status > 80) {
        return 'w-4/5 bg-greenish'
      } else if (status > 60 && status < 80) {
        return 'w-3/5 bg-greenish'
      } else if (status > 40 && status < 60) {
        return 'w-2/5 bg-yellowish'
      } else if (status > 20 && status < 40) {
        return 'w-1/5 bg-redish'
      }
    }
  }
}
</script>
<style>
.tooltip{
  visibility: hidden;
}
.has-tooltip:hover .tooltip {
  visibility: visible;
  z-index: 100;
}
</style>
