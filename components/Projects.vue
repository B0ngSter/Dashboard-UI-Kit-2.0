<template>
<div class="flex flex-row overflow-x-hidden">
    <div class="w-0 smlaptop:w-64 bg-white h-screen flex flex-col">
        <div class="ml-2 h-9 mr-2 mt-2 cursor-pointer flex flex-col items-center p-1 w-0 smlaptop:w-52">
            <div class="bg-gray-200 ml-2 h-9 mr-2 cursor-pointer flex flex-row  rounded-md items-center p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm tracking-wider pl-1 text-hardBlue">Landing Page</p>
            </div>
            <div class="ml-2 h-9 mr-2 cursor-pointer flex flex-row items-center rounded-md p-2 w-52 hover:bg-gray-300">
                <p class="font-sans text-sm tracking-wider pl-1 text-hardBlue">Strand App</p>
            </div>
        </div>
        <div class="w-60 fixed bottom-1.5 flex justify-between px-3">
            <div class="font-sans bg-gray-200 py-2 px-2 w-32 text-xs h-8">
                New Project
            </div>
            <div class="pr-3">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M3 17V19H9V17H3ZM3 5V7H13V5H3ZM13 21V19H21V17H13V15H11V21H13ZM7 9V11H3V13H7V15H9V9H7ZM21 13V11H11V13H21ZM15 9H17V7H21V5H17V3H15V9Z" fill="#110F24" fill-opacity="0.4"/>
                </svg>
            </div>
        </div>
    </div>
    <div class="w-full mt-16 smlaptop:mt-2 px-4 block h-14">
        <Head class="mt-2" />
        <div style="width: 99%;" class="rounded-md CustomMinimumH mt-6 smlaptop:mt-2 block relative my-2 chatBoxHeight bg-white">
            <div class="w-full rounded-t-xl h-14 flex flex-row items-center my-2 bg-gray-300 overflow-x-scroll smlaptop:overflow-x-hidden">
                <div style="border-bottom: 3px solid #575BDE;" class="h-full ml-3 flex items-center justify-center">
                    <p class="font-sans text-base font-medium">Overview</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Tasks</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Users</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Files</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Discussions</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Timesheets</p>
                </div>
                <div class="hoverSec cursor-pointer h-full px-3 flex items-center justify-center">
                    <p class="font-sans text-base text-gray-400">Settings</p>
                </div>
            </div>
            <div class="w-full pb-4 px-3 overflow-x-hidden flex flex-col border-b-2 border-gray-100">
                <p class="text-4xl font-bold py-4">Landing Page</p>
                <p class="text-gray-400 text-base">Giddify</p>
                <p class="text-lg font-thin tracking-wide py-3">Atom is a new plugin for Sketch, simplifying the management of modules and elements when building complex interfaces. Developed by Giddify, a landing page presents the plugin and its features in a minimal way, following the Giddify brand.</p>
                <div class="flex smlaptop:flex-row flex-col mt-1">
                    <div class="w-full smlaptop:w-1/3">
                        <p class="text-gray-400 text-sm font-semibold">Tasks Completed</p>
                        <p class="text-2xl font-semibold py-1">20%</p>
                        <div class="flex flex-row py-1 pr-2">
                            <div style="height: 5px;" class="bg-redish w-1/4 rounded-sm"></div>
                            <div style="height: 5px;" class="bg-gray-100 w-3/4 rounded-sm"></div>
                        </div>
                    </div>
                    <div class="w-full smlaptop:w-1/3">
                        <p class="text-gray-400 text-sm font-semibold">Budget</p>
                        <p class="text-2xl font-semibold py-1">75%</p>
                        <div class="flex flex-row py-1 pr-2">
                            <div style="height: 5px;" class="bg-greenish w-3/4 rounded-sm"></div>
                            <div style="height: 5px;" class="bg-gray-100 w-1/4 rounded-sm"></div>
                        </div>
                    </div>
                    <div class="w-full smlaptop:w-1/3">
                        <p class="text-gray-400 text-sm font-semibold">Deadline</p>
                        <p class="text-2xl font-semibold py-1">40%</p>
                        <div class="flex flex-row py-1 pr-2">
                            <div style="height: 5px;" class="bg-yellowish w-2/5 rounded-sm"></div>
                            <div style="height: 5px;" class="bg-gray-100 w-3/5 rounded-sm"></div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="w-full border-b-2 border-gray-100 flex justify-between py-4">
                <div class="flex flex-row">
                    <div class="lowOp">
                        <span class="material-icons px-3 pt-1">file_download_done</span>
                    </div>
                    <div>
                        <p class="text-base pt-1">Tasks</p>
                        <p class="text-sm text-gray-400">6/29 tasks completed, you’re on schedule.</p>
                    </div>
                </div>
                <div class="chip flex items-center justify-center rounded-xl mr-2">
                    <p class="py-3 px-3 text-gray-400 text-sm">1 Due soon</p>
                </div>
            </div>
            <div class="w-full border-b-2 border-gray-100 flex justify-between py-4">
                <div class="flex flex-row">
                    <div class="lowOp">
                        <span class="material-icons px-3 pt-1">account_circle</span>
                    </div>
                    <div>
                        <p class="text-base pt-1">Users</p>
                        <p class="text-sm text-gray-400">3 users currently on this project.</p>
                    </div>
                </div>
                <div>
                    <p class="pr-3 pt-3">1 Due task</p>
                </div>
            </div>
            <div class="w-full flex justify-start py-4">
                <div class="flex flex-row">
                    <div class="lowOp">
                        <span class="material-icons px-3 pt-1">file_copy</span>
                    </div>
                    <div>
                        <p class="text-base pt-1">Files</p>
                        <p class="text-sm text-gray-400">2 files have been favorited.</p>
                        <p class="text-base ">landing.zip</p>
                        <p class="text-base ">style-guide.zip</p>
                    </div>
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
  }
}
</script>

<style>
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