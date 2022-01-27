<template>
  <div class="w-full mt-16 smlaptop:mt-2 block h-screen">
      <Head class="mt-3 px-4" />
      <div class="rounded-md mx-4 mt-6 smlaptop:mt-2 block relative my-2 bg-white">
          <div class="w-full rounded-t-xl h-14 flex flex-row items-center bg-gray-300 overflow-x-scroll smlaptop:overflow-x-hidden">
              <p class="font-sans text-base font-medium pl-3 text-hardBlue">Activity</p>
          </div>
          <div class="border-b-2 border-l-2 h-auto border-gray-200  smlaptop:ml-14 ml-8" v-for="(activity, idx) in activities" :key="idx">
              <div class="h-7"></div>
              <div class="flex flex-row">
                  <div class="dot">
                      <img style="margin-left: -20px;" :src="activity.profilePic" class=" w-full rounded h-full border-2 border-gray-200" alt="">
                  </div>
                  <div class="w-11/12">
                      <div class="flex flex-row" style="margin-top: 10px;">
                          <p class="font-bold text-sm tracking-wider">{{ activity.userName }}</p>
                          <p class="text-gray-400 ml-5 text-base">{{ activity.time }}</p>
                      </div>
                      <p :class="{'mb-6': !activity.report.length}" class="text-sm tracking-wider mt-1"><span class="text-gray-400">{{ activity.description }}</span> <span class="text-sm tracking-wider text-base">{{ activity.task }}</span></p>
                      <div v-for="(task, idy) in activity.report" :key="idy">
                          <div v-if="task.type === 'checkbox'" class="flex justify-between my-4 py-3 border-2 border-gray-200 mx-2">
                              <div @click="task.checked = !task.checked" class="w-8/12 flex justify-start items-center cursor-pointer">
                                  <input type="checkbox" v-model="task.checked" class="focus:outline-none cursor-pointer rounded-md bg-gray-300 h-4 w-4 ml-3" placeholder="Add task...">
                                  <strike class="font-sans pl-4 text-gray-400 cursor-pointer tracking-wider text-sm text-hardBlue" v-if="task.checked">{{ task.message }}</strike>
                                  <p v-else class="font-sans cursor-pointer text-sm tracking-wider pl-3 pt-1 ">{{ task.message }}</p>
                              </div>
                              <div class=" w-4/12">
                                  <div @click="task.highLight = !task.highLight" v-if="task.highLight" class="w-1/12 flex justify-end cursor-pointer float-right mr-4">
                                      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                      <path fill-rule="evenodd" clip-rule="evenodd" d="M21.3333 0H2.66667C1.18667 0 0 1.2 0 2.66667V21.3333C0 22.8 1.18667 24 2.66667 24H21.3333C22.8133 24 24 22.8 24 21.3333V2.66667C24 1.2 22.8133 0 21.3333 0ZM12 16.216L16.944 19.2L15.632 13.576L20 9.792L14.248 9.304L12 4L9.752 9.304L4 9.792L8.368 13.576L7.056 19.2L12 16.216Z" fill="#575BDE"/>
                                      </svg>
                                  </div>
                                  <div @click="task.highLight = !task.highLight" v-else class="w-1/12 flex justify-end cursor-pointer float-right mr-4">
                                      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                      <path fill-rule="evenodd" clip-rule="evenodd" d="M21.3333 0H2.66667C1.18667 0 0 1.2 0 2.66667V21.3333C0 22.8 1.18667 24 2.66667 24H21.3333C22.8133 24 24 22.8 24 21.3333V2.66667C24 1.2 22.8133 0 21.3333 0ZM12 16.216L16.944 19.2L15.632 13.576L20 9.792L14.248 9.304L12 4L9.752 9.304L4 9.792L8.368 13.576L7.056 19.2L12 16.216Z" fill="#ECECEE"/>
                                      </svg>
                                  </div>
                              </div>
                          </div>
                          <div v-if="task.type === 'Zip'" class="flex justify-start my-4 py-3 border-2 border-gray-200 mx-2">
                              <div class="flex justify-start items-center cursor-pointer">
                                  <div class="lowOp">
                                      <span class="material-icons px-3 pt-1">insert_drive_file</span>
                                  </div>
                                  <div class="flex flex-col">
                                      <p class="tracking-wider text-sm">{{ task.name }}</p>
                                      <p class="text-gray-400 tracking-wider text-sm">{{ task.type }}</p>
                                  </div>
                              </div>
                              <div class="w-1/5 flex justify-start">
                                  <div @click="task.highLight = !task.highLight" v-if="task.highLight" class="w-1/12 flex justify-end cursor-pointer float-right ml-4">
                                      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                      <path fill-rule="evenodd" clip-rule="evenodd" d="M21.3333 0H2.66667C1.18667 0 0 1.2 0 2.66667V21.3333C0 22.8 1.18667 24 2.66667 24H21.3333C22.8133 24 24 22.8 24 21.3333V2.66667C24 1.2 22.8133 0 21.3333 0ZM12 16.216L16.944 19.2L15.632 13.576L20 9.792L14.248 9.304L12 4L9.752 9.304L4 9.792L8.368 13.576L7.056 19.2L12 16.216Z" fill="#575BDE"/>
                                      </svg>
                                  </div>
                                  <div @click="task.highLight = !task.highLight" v-else class="w-1/12 flex justify-end cursor-pointer float-right ml-4">
                                      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                      <path fill-rule="evenodd" clip-rule="evenodd" d="M21.3333 0H2.66667C1.18667 0 0 1.2 0 2.66667V21.3333C0 22.8 1.18667 24 2.66667 24H21.3333C22.8133 24 24 22.8 24 21.3333V2.66667C24 1.2 22.8133 0 21.3333 0ZM12 16.216L16.944 19.2L15.632 13.576L20 9.792L14.248 9.304L12 4L9.752 9.304L4 9.792L8.368 13.576L7.056 19.2L12 16.216Z" fill="#ECECEE"/>
                                      </svg>
                                  </div>
                              </div>
                          </div>
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
  },
  data () {
    return {
      activities: [
        {
          userName: 'Camilla Tunney',
          profilePic: 'https://i.pinimg.com/originals/08/53/8a/08538a67eeb68a5fba7586ed18b6386f.jpg',
          time: '17:32',
          description: 'Created two new tasks.',
          task: '#landing-page',
          report: [
            {
              type: 'checkbox',
              message: 'Send prototype to team',
              highLight: true,
              checked: false
            },
            {
              type: 'checkbox',
              message: 'Review content with copywriter',
              highLight: false,
              checked: false
            }
          ]
        },
        {
          userName: 'Felix Levan',
          profilePic: 'https://64.media.tumblr.com/0f1d9be0930e0fd6e1421e0af63b4baa/4b38c49aa49bf456-a5/s1280x1920/54be3df4f578d67626ed9b3849f53d129667b940.jpg',
          time: '17:29',
          description: 'Favorited "landing.zip".',
          task: '#landing-page',
          report: [
          ]
        },
        {
          userName: 'Felix Levan',
          profilePic: 'https://64.media.tumblr.com/0f1d9be0930e0fd6e1421e0af63b4baa/4b38c49aa49bf456-a5/s1280x1920/54be3df4f578d67626ed9b3849f53d129667b940.jpg',
          time: '17:28',
          description: 'Uploaded a new file.',
          task: '#landing-page',
          report: [
            {
              type: 'Zip',
              name: 'landing.zip',
              highLight: true
            }
          ]
        },
        {
          userName: 'Kristopher Fager',
          profilePic: 'https://i.imgur.com/RM2ln57.jpg',
          time: '17:32',
          description: 'Marked task as complete.',
          task: '#strand-app',
          report: [
            {
              type: 'checkbox',
              message: 'Change logo from png to svg',
              highLight: false,
              checked: true
            }
          ]
        }
      ]
    }
  },
  methods: {
  }
}
</script>

<style>
.dot{
    width: 40px;
    top: 100px;
    height: 40px;
    border-radius:7px;
}

.line{
    height:103px;
    width:2px;
    background: #D1D6E6;
    margin-left:5.3px;
}
.lowOp {
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
.lowOp {
    opacity: 0.5;
}
</style>
