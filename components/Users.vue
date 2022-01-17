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
    <div class="w-full mt-16 smlaptop:mt-2 px-4 block h-14">
        <Head class="mt-3" />
        <div style="width: 99%;" class="rounded-md CustomMinimumH mt-6 smlaptop:mt-2 block relative my-2 chatBoxHeight bg-white">
            <div class="w-full rounded-t-xl h-14 flex flex-row items-center my-2 bg-gray-300 overflow-x-scroll smlaptop:overflow-x-hidden">
                <p class="font-sans text-base font-medium pl-3">Kristopher Fager</p>
            </div>
            <div class="mx-4">
                <p class="font-sans text-base font-medium">Name:</p>
                <input type="text" class="focus:outline-none font-sm rounded-sm border-gray-100 border-2 bg-gray-300 h-9 mt-1 pl-3 w-full smlaptop:w-1/3" value="Kristopher Fager">
            </div>
            <div class="mx-4 mt-2">
                <p class="font-sans text-base font-medium">Email:</p>
                <input type="text" class="focus:outline-none font-sm rounded-sm border-gray-100 border-2 bg-gray-300 h-9 mt-1 pl-3 w-full smlaptop:w-1/3" value="kristopher.fager@example.com">
                <p class="font-sans text-xs text-gray-400 font-sm mt-2">Email will not be publicly displayed.</p>
            </div>
            <div class="mt-4 block mx-4">
                <p class="font-sans text-base font-medium">Role:</p>
                <div class="flex flex-row mt-4">
                    <input type="checkbox" class="focus:outline-none cursor-pointer rounded-full bg-gray-300 h-5 w-5 blackout">
                    <div class="flex flex-col ml-3">
                        <p class="font-sans text-base font-sm">Admin</p>
                        <p class="font-sans text-sm text-gray-400 font-sm">Full access to all features and account settings.</p>
                    </div>
                </div>
                <div class="flex flex-row mt-4">
                    <input type="checkbox" checked class="focus:outline-none cursor-pointer rounded-full bg-hardBlue h-5 w-5 blackout">
                    <div class="flex flex-col ml-3">
                        <p class="font-sans text-base font-sm">Editor</p>
                        <p class="font-sans text-sm text-gray-400 font-sm">Access to all features except from managing the account.</p>
                    </div>
                </div>
                <div class="flex flex-row mt-4">
                    <input type="checkbox" class="focus:outline-none cursor-pointer rounded-full bg-gray-300 h-5 w-5 blackout">
                    <div class="flex flex-col ml-3">
                        <p class="font-sans text-base font-sm">Viewer</p>
                        <p class="font-sans text-sm text-gray-400 font-sm">Can only view projects and downloud files.</p>
                    </div>
                </div>
            </div>
            <div class="mt-4 block mx-4">
                <p class="font-sans text-base font-medium">Projects:</p>
                <div class="px-4 py-4 mt-3 w-full flex flex-row items-center border-gray-100 border-2">
                    <div class="block w-1/2">
                        <p class="font-sans text-base font-sm">Flowchart Editor</p>
                        <p class="font-sans text-sm text-gray-400 font-sm">Enigm</p>
                    </div>
                    <div class="w-1/2">
                        <select name="cars" class="mr-3 text-hardBlue focus:outline-none cursor-pointer bg-gray-300 w-2/3 h-9 px-4 border border-gray-200" id="cars">
                            <option>Edit</option>
                            <option>View</option>
                            <option>Hide</option>
                        </select>
                    </div>
                </div>
                <div class="px-4 py-4 w-full flex flex-row items-center border-gray-100 border-b-2 border-r-2 border-l-2">
                    <div class="block w-1/2">
                        <p class="font-sans text-base font-sm">Landing Page</p>
                        <p class="font-sans text-sm text-gray-400 font-sm">Giddify</p>
                    </div>
                    <div class="w-1/2">
                        <select name="cars" class="mr-3 text-hardBlue focus:outline-none cursor-pointer bg-gray-300 w-2/3 h-9 px-4 border border-gray-200" id="cars">
                            <option>Edit</option>
                            <option>View</option>
                            <option>Hide</option>
                        </select>
                    </div>
                </div>
                <div class="px-4 py-4 w-full flex flex-row items-center border-gray-100 border-b-2 border-r-2 border-l-2">
                    <div class="block w-1/2">
                        <p class="font-sans text-base font-sm">Strand App</p>
                        <p class="font-sans text-sm text-gray-400 font-sm">Mondemi</p>
                    </div>
                    <div class="w-1/2">
                        <select name="cars" class="mr-3 text-hardBlue focus:outline-none cursor-pointer bg-gray-300 w-2/3 h-9 px-4 border border-gray-200" id="cars">
                            <option>Edit</option>
                            <option>View</option>
                            <option>Hide</option>
                        </select>
                    </div>
                </div>
            </div>
            <div class="mx-4">
                <div class="w-full flex justify-center items-center bg-blueish mt-3 h-16 mb-5 rounded-sm text-white cursor-pointer">
                    Save Changes
                </div>
            </div>
            <div class="h-2 w-full" />
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