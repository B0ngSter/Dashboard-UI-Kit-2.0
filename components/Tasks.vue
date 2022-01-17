<template>
<div class="flex flex-row h-auto overflow-x-hidden">
    <div class="w-0 relative smlaptop:w-72 bg-white h-auto min-h-screen overflow-hidden block">
        <div class="ml-2 h-9 mr-2 mt-2 cursor-pointer flex flex-col items-center p-1 w-52">
            <div class="bg-gray-200 ml-2 h-9 mr-2 cursor-pointer flex flex-row  rounded-md items-center p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm pl-1 text-sm">Inbox</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer border-b-2 border-gray-100 flex flex-row items-center rounded-md p-2 w-52 hover:bg-gray-300 ">
                <p class="font-sans text-sm pl-1 text-base">All</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer flex flex-row items-center rounded-md p-2 pt-3 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm pl-1 text-base">Starred</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer flex flex-row items-center rounded-md p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm pl-1 text-base">Forecast</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer flex flex-row items-center rounded-md p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm pl-1 text-base">Completed</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer flex flex-row items-center rounded-md p-2 pt-3 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm pl-1 text-gray-400 text-base">MY LISTS</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer flex flex-row items-center rounded-md p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm pl-1 text-base">Landing Page</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer flex flex-row items-center rounded-md p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm pl-1 text-base">Floychart Editor</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer flex flex-row items-center rounded-md p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm pl-1 text-base">Strand App</p>
            </div>
        </div>
        <div class="w-60 absolute bottom-1.5 flex justify-between px-3">
            <div class="font-sans bg-gray-200 py-2 px-2 w-32 text-xs h-8">
                New List
            </div>
            <div class="pr-3">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M3 17V19H9V17H3ZM3 5V7H13V5H3ZM13 21V19H21V17H13V15H11V21H13ZM7 9V11H3V13H7V15H9V9H7ZM21 13V11H11V13H21ZM15 9H17V7H21V5H17V3H15V9Z" fill="#110F24" fill-opacity="0.4"/>
                </svg>
            </div>
        </div>
    </div>
    <div class="w-full mt-16 smlaptop:mt-2 px-2 block h-14">
        <Head class="mt-3" />
        <div style="width: 99%;" class="rounded-md CustomMinimumH mt-6 smlaptop:mt-2 block relative my-2 chatBoxHeight bg-white">
            <div class="w-full rounded-t-xl h-14 flex flex-row items-center my-2 bg-gray-300 overflow-x-scroll smlaptop:overflow-x-hidden">
                <p class="font-sans text-base font-medium pl-3 text-hardBlue">Inbox</p>
            </div>
            <div class="flex justify-start pt-2 mx-2 border-b-2 border-gray-100">
                <input type="text" v-model="enteredTask" class="focus:outline-none border-2 border-gray-100 rounded-sm bg-gray-300 h-10 ml-2 pl-4 placeholder:text-gray-400 w-full" @keyup="addTask($event)" placeholder="Add task...">
                <div class="h-14 mt-1 blackout">
                    <span class="material-icons px-3 pt-1 h-14">calendar_month</span>
                </div>
            </div>
            <div class="flex justify-start my-2 mx-2 pb-4 border-b-2 border-gray-100" v-for="(task, i) in tasks" :key="i">
                <div @click="task.checked = !task.checked" class="w-8/12 flex justify-start items-center cursor-pointer">
                    <input type="checkbox" v-model="task.checked" class="focus:outline-none cursor-pointer rounded-md bg-gray-300 h-5 w-5 blackout ml-3" placeholder="Add task...">
                    <strike class="font-sans pl-4 pt-1 text-gray-400 cursor-pointer text-sm text-hardBlue" v-if="task.checked">{{ task.taskName }}</strike>
                    <p v-else class="font-sans cursor-pointer text-sm tracking-wider pl-3 pt-1">{{ task.taskName }}</p>
                </div>
                <div class="w-2/12 text-sm text-gray-400">{{ task.due }}</div>
                <div v-if="task.pinned" class="w-1/12 flex justify-end">
                    <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd" clip-rule="evenodd" d="M11 3.99999V11.6667C11 13.14 9.80669 14.3333 8.33335 14.3333C6.86002 14.3333 5.66669 13.14 5.66669 11.6667V3.33332C5.66669 2.41332 6.41335 1.66666 7.33335 1.66666C8.25335 1.66666 9.00002 2.41332 9.00002 3.33332V10.3333C9.00002 10.7 8.70002 11 8.33335 11C7.96669 11 7.66669 10.7 7.66669 10.3333V3.99999H6.66669V10.3333C6.66669 11.2533 7.41335 12 8.33335 12C9.25335 12 10 11.2533 10 10.3333V3.33332C10 1.85999 8.80669 0.666656 7.33335 0.666656C5.86002 0.666656 4.66669 1.85999 4.66669 3.33332V11.6667C4.66669 13.6933 6.30669 15.3333 8.33335 15.3333C10.36 15.3333 12 13.6933 12 11.6667V3.99999H11Z" fill="#110F24" fill-opacity="0.4"/>
                    </svg>
                </div>
                <div v-else class="w-1/12 flex justify-end" />
                <div @click="toDoList[i].bookmark = !toDoList[i].bookmark" v-if="task.bookmark" class="w-1/12 mr-3 flex justify-end cursor-pointer">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd" clip-rule="evenodd" d="M21.3333 0H2.66667C1.18667 0 0 1.2 0 2.66667V21.3333C0 22.8 1.18667 24 2.66667 24H21.3333C22.8133 24 24 22.8 24 21.3333V2.66667C24 1.2 22.8133 0 21.3333 0ZM12 16.216L16.944 19.2L15.632 13.576L20 9.792L14.248 9.304L12 4L9.752 9.304L4 9.792L8.368 13.576L7.056 19.2L12 16.216Z" fill="#575BDE"/>
                    </svg>
                </div>
                <div @click="toDoList[i].bookmark = !toDoList[i].bookmark" v-else class="w-1/12 mr-3 flex justify-end cursor-pointer">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd" clip-rule="evenodd" d="M21.3333 0H2.66667C1.18667 0 0 1.2 0 2.66667V21.3333C0 22.8 1.18667 24 2.66667 24H21.3333C22.8133 24 24 22.8 24 21.3333V2.66667C24 1.2 22.8133 0 21.3333 0ZM12 16.216L16.944 19.2L15.632 13.576L20 9.792L14.248 9.304L12 4L9.752 9.304L4 9.792L8.368 13.576L7.056 19.2L12 16.216Z" fill="#ECECEE"/>
                    </svg>
                </div>
            </div>
        </div>
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
        tasks: [
            {
                checked: false,
                due: 'Today',
                bookmark: false,
                pinned: true,
                taskName: 'Send prototype to team'
            },
            {
                checked: false,
                due: 'Today',
                bookmark: false,
                pinned: false,
                taskName: 'Review content with copywriter'
            },
            {
                checked: true,
                due: 'Today',
                bookmark: true,
                pinned: true,
                taskName: 'Optimize hero images'
            },
            {
                checked: true,
                due: 'Today',
                bookmark: false,
                pinned: true,
                taskName: 'Add loading screen after sign up'
            },
            {
                checked: false,
                due: 'Today',
                bookmark: false,
                pinned: true,
                taskName: 'Get file structure ready for cms'
            },
            {
                checked: false,
                due: 'Today',
                pinned: false,
                bookmark: true,
                taskName: 'Update style guide  with new colors'
            },
            {
                checked: true,
                due: 'Today',
                bookmark: true,
                pinned: false,
                taskName: 'Define grid for editor'
            },
            {
                checked: true,
                due: 'Today',
                bookmark: false,
                pinned: false,
                taskName: 'Fix footer on mobile'
            }
        ],
        enteredTask: ''
    }
  },
  methods: {
      addTask (event) {
          if (event.keyCode === 13) {
            event.preventDefault()
            if (this.enteredTask.length) {
                const dict = {
                    checked: false,
                    taskName: this.enteredTask
                }
                this.tasks.push(dict)
                this.enteredTask = ''
            }
          }
      }
  }
}
</script>

<style>
.lowOp {
    opacity: 0.5;
}
.blackout {
    filter: grayscale(100%);
    opacity: 0.5;
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