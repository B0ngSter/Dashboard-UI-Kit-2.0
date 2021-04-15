<template>
  <div class="container">
    <div class="flex w-screen">
      <div class="w-0 smlaptop:w-72 bg-DarkBlue h-screen flex-none">
        <div class="container px-5">
          <div class="flex content-center mt-5">
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
          <div class="mt-3">
            <p class="font-sans font-bold text-xs text-gray-400 pl-2">MAIN</p>
          </div>
          <div :class="{'bg-activeBlue': activeTab === 'Home'}" class="flex rounded content-center my-auto cursor-pointer py-1 mt-1 hover:bg-hoverBlue" @click="activeTab = 'Home'">
            <div class="pl-1">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M3 13H11V3H3V13ZM3 21H11V15H3V21ZM13 21H21V11H13V21ZM13 3V9H21V3H13Z" fill="white"/>
              </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">HOME</p>
            </div>
          </div>
          <div class="flex content-center my-auto py-1 mt-1 rounded cursor-pointer hover:bg-hoverBlue">
            <div class="pl-1">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M3 17H21V15H3V17ZM3 20H21V19H3V20ZM3 13H21V10H3V13ZM3 4V8H21V4H3Z" fill="white"/>
              </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">Activity</p>
            </div>
          </div>
          <div class="flex content-center my-auto py-1 mt-1 rounded cursor-pointer hover:bg-hoverBlue">
            <div class="pl-1">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M20 6H12L10 4H4C2.9 4 2.01 4.9 2.01 6L2 18C2 19.1 2.9 20 4 20H20C21.1 20 22 19.1 22 18V8C22 6.9 21.1 6 20 6ZM20 18H4V8H20V18Z" fill="white"/>
              </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">Projects</p>
            </div>
          </div>
          <div class="flex content-center my-auto py-1 mt-1 rounded cursor-pointer hover:bg-hoverBlue">
            <div class="pl-1">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M18 7.00009L16.59 5.59009L10.25 11.9301L11.66 13.3401L18 7.00009ZM22.24 5.59009L11.66 16.1701L7.48003 12.0001L6.07003 13.4101L11.66 19.0001L23.66 7.00009L22.24 5.59009ZM0.410034 13.4101L6.00003 19.0001L7.41003 17.5901L1.83003 12.0001L0.410034 13.4101Z" fill="white"/>
              </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">Tasks</p>
            </div>
          </div>
          <div class="mt-3">
            <p class="font-sans text-xs font-bold text-gray-300 pl-2">PEOPLE</p>
          </div>
          <div class="flex content-center my-auto py-1 mt-1 rounded cursor-pointer hover:bg-hoverBlue">
            <div class="pl-1">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M16.5 12C17.88 12 18.99 10.88 18.99 9.5C18.99 8.12 17.88 7 16.5 7C15.12 7 14 8.12 14 9.5C14 10.88 15.12 12 16.5 12ZM9 11C10.66 11 11.99 9.66 11.99 8C11.99 6.34 10.66 5 9 5C7.34 5 6 6.34 6 8C6 9.66 7.34 11 9 11ZM16.5 14C14.67 14 11 14.92 11 16.75V19H22V16.75C22 14.92 18.33 14 16.5 14ZM9 13C6.67 13 2 14.17 2 16.5V19H9V16.75C9 15.9 9.33 14.41 11.37 13.28C10.5 13.1 9.66 13 9 13Z" fill="white"/>
              </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">Customers</p>
            </div>
          </div>
          <div :class="{'bg-activeBlue': activeTab === 'Convo'}" class="flex mt-1 content-center my-auto py-1 rounded cursor-pointer hover:bg-hoverBlue" @click="OpenConversation()">
            <div class="pl-1">
             <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M21.99 4C21.99 2.9 21.1 2 20 2H4C2.9 2 2 2.9 2 4V16C2 17.1 2.9 18 4 18H18L22 22L21.99 4ZM18 14H6V12H18V14ZM18 11H6V9H18V11ZM18 8H6V6H18V8Z" fill="white"/>
            </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">Conversations</p>
            </div>
          </div>
          <div class="mt-3">
            <p class="font-sans text-xs cursor-pointer font-bold text-gray-300 pl-2">ACCOUNT</p>
          </div>
          <div class="flex content-center my-auto py-1 mt-1 rounded cursor-pointer hover:bg-hoverBlue">
            <div class="pl-1">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM12 5C13.66 5 15 6.34 15 8C15 9.66 13.66 11 12 11C10.34 11 9 9.66 9 8C9 6.34 10.34 5 12 5ZM12 19.2C9.5 19.2 7.29 17.92 6 15.98C6.03 13.99 10 12.9 12 12.9C13.99 12.9 17.97 13.99 18 15.98C16.71 17.92 14.5 19.2 12 19.2Z" fill="white"/>
              </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">Users</p>
            </div>
          </div>
          <div class="flex content-center my-auto py-1 mt-1 rounded cursor-pointer hover:bg-hoverBlue">
            <div class="pl-1">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M19.43 12.98C19.47 12.66 19.5 12.34 19.5 12C19.5 11.66 19.47 11.34 19.43 11.02L21.54 9.37C21.73 9.22 21.78 8.95 21.66 8.73L19.66 5.27C19.54 5.05 19.27 4.97 19.05 5.05L16.56 6.05C16.04 5.65 15.48 5.32 14.87 5.07L14.49 2.42C14.46 2.18 14.25 2 14 2H9.99996C9.74996 2 9.53996 2.18 9.50996 2.42L9.12996 5.07C8.51996 5.32 7.95996 5.66 7.43996 6.05L4.94996 5.05C4.71996 4.96 4.45996 5.05 4.33996 5.27L2.33996 8.73C2.20996 8.95 2.26996 9.22 2.45996 9.37L4.56996 11.02C4.52996 11.34 4.49996 11.67 4.49996 12C4.49996 12.33 4.52996 12.66 4.56996 12.98L2.45996 14.63C2.26996 14.78 2.21996 15.05 2.33996 15.27L4.33996 18.73C4.45996 18.95 4.72996 19.03 4.94996 18.95L7.43996 17.95C7.95996 18.35 8.51996 18.68 9.12996 18.93L9.50996 21.58C9.53996 21.82 9.74996 22 9.99996 22H14C14.25 22 14.46 21.82 14.49 21.58L14.87 18.93C15.48 18.68 16.04 18.34 16.56 17.95L19.05 18.95C19.28 19.04 19.54 18.95 19.66 18.73L21.66 15.27C21.78 15.05 21.73 14.78 21.54 14.63L19.43 12.98ZM12 15.5C10.07 15.5 8.49996 13.93 8.49996 12C8.49996 10.07 10.07 8.5 12 8.5C13.93 8.5 15.5 10.07 15.5 12C15.5 13.93 13.93 15.5 12 15.5Z" fill="white"/>
              </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">Settings</p>
            </div>
          </div>
          <div class="mt-3">
            <p class="font-sans text-xs font-bold text-gray-300 pl-2">MISC</p>
          </div>
          <div class="flex content-center my-auto py-1 mt-1 rounded cursor-pointer hover:bg-hoverBlue">
            <div class="pl-1">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M12 2C8.14 2 5 5.14 5 9C5 14.25 12 22 12 22C12 22 19 14.25 19 9C19 5.14 15.86 2 12 2ZM12.88 15.75H11.13V14H12.88V15.75ZM12.88 12.88H11.13C11.13 10.04 13.75 10.26 13.75 8.5C13.75 7.54 12.96 6.75 12 6.75C11.04 6.75 10.25 7.54 10.25 8.5H8.5C8.5 6.57 10.07 5 12 5C13.93 5 15.5 6.57 15.5 8.5C15.5 10.69 12.88 10.91 12.88 12.88Z" fill="white"/>
              </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">Empty State</p>
            </div>
          </div>
          <div class="flex content-center my-auto py-1 mt-1 rounded cursor-pointer hover:bg-hoverBlue">
            <div class="pl-1">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.9" fill-rule="evenodd" clip-rule="evenodd" d="M18 8H17V6C17 3.24 14.76 1 12 1C9.24 1 7 3.24 7 6V8H6C4.9 8 4 8.9 4 10V20C4 21.1 4.9 22 6 22H18C19.1 22 20 21.1 20 20V10C20 8.9 19.1 8 18 8ZM12 17C10.9 17 10 16.1 10 15C10 13.9 10.9 13 12 13C13.1 13 14 13.9 14 15C14 16.1 13.1 17 12 17ZM15.1 8H8.9V6C8.9 4.29 10.29 2.9 12 2.9C13.71 2.9 15.1 4.29 15.1 6V8Z" fill="white"/>
              </svg>
            </div>
            <div class="flex-initial flex items-center pl-2">
              <p class="font-sans text-sm font-normal text-white">Onboarding</p>
            </div>
          </div>
        </div>
      </div>
      <div v-if="activeTab === 'Convo'" class="w-0 smlaptop:w-72 bg-white h-screen flex flex-col">
        <div v-for="(user, idy) in ChatJson" :key="idy" class="ml-2 mr-2 mt-2 cursor-pointer flex flex-row items-center p-1 w-52 hover:bg-gray-200" @click="OpenChat(idy)">
          <img :src="user.profilePic" class="w-6" alt="">
          <p class="font-sans text-sm pl-1" :class="{'font-bold': user.newMessages}">{{ user.userName }}</p>
        </div>
        <div class="w-60 fixed bottom-1.5 flex justify-between px-3">
          <div class="font-sans bg-gray-200 py-2 px-2 w-32 text-xs h-8">
            New Conversation
          </div>
          <div class="pr-3">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path fill-rule="evenodd" clip-rule="evenodd" d="M3 17V19H9V17H3ZM3 5V7H13V5H3ZM13 21V19H21V17H13V15H11V21H13ZM7 9V11H3V13H7V15H9V9H7ZM21 13V11H11V13H21ZM15 9H17V7H21V5H17V3H15V9Z" fill="#110F24" fill-opacity="0.4"/>
            </svg>
          </div>
        </div>
      </div>
      <div v-if="activeTab === 'Convo'" class="w-full overflow-x-hidden bg-gray-200 h-screen">
        <div class="w-full fixed smlaptop:hidden  z-10 bg-DarkBlue p-4 flex justify-between items-center">
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
          <div class="burger">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path fill-rule="evenodd" clip-rule="evenodd" d="M3 18H21V16H3V18ZM3 13H21V11H3V13ZM3 6V8H21V6H3Z" fill="white"/>
            </svg>
          </div>
        </div>
        <div class="">
          <div class="w-auto mt-2 px-2 flex items-center justify-between h-14">
            <div class="flex h-8 rounded justify-start bg-white items-center">
              <div class="pl-2">
                <svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M11.625 10.5H11.0325L10.8225 10.2975C11.5575 9.4425 12 8.3325 12 7.125C12 4.4325 9.8175 2.25 7.125 2.25C4.4325 2.25 2.25 4.4325 2.25 7.125C2.25 9.8175 4.4325 12 7.125 12C8.3325 12 9.4425 11.5575 10.2975 10.8225L10.5 11.0325V11.625L14.25 15.3675L15.3675 14.25L11.625 10.5ZM7.125 10.5C5.2575 10.5 3.75 8.9925 3.75 7.125C3.75 5.2575 5.2575 3.75 7.125 3.75C8.9925 3.75 10.5 5.2575 10.5 7.125C10.5 8.9925 8.9925 10.5 7.125 10.5Z" fill="#110F24" fill-opacity="0.4"/>
                </svg>
              </div>
              <div>
                <input type="text" class="focus:outline-none" placeholder="Search...">
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
          <div v-if="activeTab === 'Convo' && !isMobileDevice" class="w-auto bg-white mt-4 m-2 flex items-center justify-between smlaptop:hidden h-14">
            <div class="w-4/5">
              <img :src="previewChat.profilePic" class="w-6 pl-2 float-left mr-2" alt="">
              <p class="font-sans text-base font-bold">{{ previewChat.userName }}</p>
            </div>
            <div class="w-1/5">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd" clip-rule="evenodd" d="M13.9654 19C13.9049 18.9958 13.8895 18.9964 13.8296 18.986C13.6949 18.9628 13.5653 18.9117 13.451 18.8367C13.3932 18.7988 13.3428 18.7547 13.2924 18.7077L7.29211 12.7074C7.25071 12.6631 7.23916 12.653 7.20241 12.6045C7.16116 12.5501 7.12551 12.4915 7.09615 12.4298C6.96795 12.1602 6.96795 11.8403 7.09615 11.5708C7.12551 11.5091 7.16116 11.4504 7.20241 11.396C7.23916 11.3476 7.25071 11.3375 7.29211 11.2932L13.2924 5.29291C13.3367 5.25151 13.3469 5.23991 13.3953 5.20321C13.5224 5.10675 13.6724 5.04165 13.8296 5.0145C13.9418 4.9952 14.0572 4.9952 14.1695 5.0145C14.2592 5.03 14.3468 5.0578 14.429 5.0969C14.7414 5.24546 14.9589 5.55362 14.9943 5.89774C15.0083 6.03374 14.994 6.17225 14.9527 6.30256C14.9182 6.41111 14.8652 6.51356 14.7964 6.60427C14.7596 6.65272 14.7481 6.66282 14.7067 6.70717L9.41355 12.0003L14.7067 17.2934L14.7533 17.3433C14.7915 17.3903 14.8024 17.4013 14.8357 17.4521C14.8982 17.5473 14.9442 17.6531 14.9711 17.7637C14.9927 17.8523 15.0021 17.9437 14.999 18.0347C14.9872 18.3804 14.7912 18.7027 14.4897 18.8722C14.3904 18.928 14.2817 18.9667 14.1695 18.986C14.1096 18.9964 14.0942 18.9958 14.0337 19C14.0109 19 13.9881 19 13.9654 19Z" fill="#110F24" fill-opacity="0.4"/>
              </svg>
            </div>
          </div>
          <div class="rounded-xl CustomMinimumH block relative m-2 chatBoxHeight bg-white">
            <div class="w-full rounded-t-xl h-10 flex justify-start items-center my-2 bg-gray-300">
              <p class="font-sans text-base font-bold pl-3">{{ previewChat.userName }}</p>
            </div>
            <div class="w-full px-3 py-5 overflow-x-hidden flex flex-col">
              <div v-for="(chat, idx) in previewChat.chatHistory" :key="idx" class="flex flex-col w-full">
                <div v-if="chat.sender === 'Me'" class="mt-5">
                  <div class="flex items-center">
                    <img src="@/static/Profile6.png" class="w-6 float-left" alt="">
                    <p class="font-sans pl-2 text-base font-bold">Felix Levan<span class="text-gray-400 pl-2 font-normal text-base ">{{ chat.time }}</span></p>
                  </div>
                  <p class="font-sans pl-8 font-normal text-base">{{ chat.message }}</p>
                  <img v-if="chat.img" class="rounded-md ml-8 w-1/5" :src="chat.img" alt="">
                </div>
                <div v-if="chat.sender === 'notMe'" class="mt-5">
                  <div class="flex items-center">
                    <img :src="previewChat.profilePic" class="w-6 float-left" alt="">
                    <p class=" font-sans pl-2 text-base font-bold">{{ previewChat.userName }}<span class="text-gray-400 pl-2 font-normal text-base ">{{ chat.time }}</span></p>
                  </div>
                  <p class="font-sans pl-8 font-normal text-base">{{ chat.message }}</p>
                  <img v-if="chat.img" class="rounded-md ml-8 w-1/5" :src="chat.img" alt="">
                </div>
              </div>
              <h2 v-if="previewChat.newMessages" class="text-center relative z-10"><span class="line-center">New Messages</span></h2>
              <div v-if="previewChat.newMessages" class="mt-5">
                <div class="flex items-center">
                  <img :src="previewChat.profilePic" class="w-6 float-left" alt="">
                  <p class=" font-sans pl-2 text-base font-bold">{{ previewChat.userName }}<span class="text-gray-400 pl-2 text-base ">{{ previewChat.newMessages.time }}</span></p>
                </div>
                <p class="font-sans pl-8 text-base">{{ previewChat.newMessages.message }}</p>
                <img v-if="previewChat.newMessages.img" class="rounded-md ml-8 w-1/5" :src="chat.img" alt="">
              </div>
            </div>
            <div class="w-full absolute bottom-3 flex items-end px-3">
              <div class="bg-gray-200 py-2 px-2 flex-grow text-xs h-8">
                <input class="bg-gray-200 w-11/12 focus:outline-none" v-model="writtenMessage" @keydown="sendMessage($event)" placeholder="Message..." type="text">
              </div>
              <div class="pr-3 h-8 pl-2 flex items-center">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M12 5C11.4477 5 11 5.44772 11 6V11H6C5.44772 11 5 11.4477 5 12C5 12.5523 5.44772 13 6 13H11V18C11 18.5523 11.4477 19 12 19C12.5523 19 13 18.5523 13 18V13H18C18.5523 13 19 12.5523 19 12C19 11.4477 18.5523 11 18 11H13V6C13 5.44772 12.5523 5 12 5Z" fill="#110F24" fill-opacity="0.4"/>
                </svg>
              </div>
              <div class="pr-3 h-8 flex items-center">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M11.99 2C6.47 2 2 6.48 2 12C2 17.52 6.47 22 11.99 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 11.99 2ZM12 20C7.58 20 4 16.42 4 12C4 7.58 7.58 4 12 4C16.42 4 20 7.58 20 12C20 16.42 16.42 20 12 20ZM15.5 11C16.33 11 17 10.33 17 9.5C17 8.67 16.33 8 15.5 8C14.67 8 14 8.67 14 9.5C14 10.33 14.67 11 15.5 11ZM8.5 11C9.33 11 10 10.33 10 9.5C10 8.67 9.33 8 8.5 8C7.67 8 7 8.67 7 9.5C7 10.33 7.67 11 8.5 11ZM12 17.5C14.33 17.5 16.31 16.04 17.11 14H6.89C7.69 16.04 9.67 17.5 12 17.5Z" fill="#110F24" fill-opacity="0.4"/>
                </svg>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div v-if="activeTab === 'Home'" class="w-full bg-gray-200 h-screen">
        <Home />
      </div>
    </div>
  </div>
</template>

<script>
import Home from '~/components/Home'
export default {
  components: {
    Home
  },
  data () {
    return {
      writtenMessage: '',
      previewChat: {},
      ChatJson: [
        {
          userName: 'Camilla Tunney',
          profilePic: 'https://i.pinimg.com/originals/08/53/8a/08538a67eeb68a5fba7586ed18b6386f.jpg',
          newMessages: null,
          chatHistory: [
            {
              sender: 'notMe',
              message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime mollitia, molestiae quas vel sint commodi',
              time: '10:35',
              img: null
            },
            {
              sender: 'Me',
              message: 'Lorem ipsum',
              time: '10:37',
              img: null
            },
            {
              sender: 'notMe',
              message: 'dolor sit sint commodi',
              time: '10:41',
              img: null
            }
          ]
        },
        {
          userName: 'Alise Stoke',
          profilePic: 'https://64.media.tumblr.com/0f1d9be0930e0fd6e1421e0af63b4baa/4b38c49aa49bf456-a5/s1280x1920/54be3df4f578d67626ed9b3849f53d129667b940.jpg',
          newMessages: null,
          chatHistory: [
            {
              sender: 'notMe',
              message: 'yo!! what up',
              time: '10:35',
              img: null
            },
            {
              sender: 'Me',
              message: 'all good man!',
              time: '10:37',
              img: null
            },
            {
              sender: 'notMe',
              message: 'check this out',
              time: '10:41',
              img: 'https://images-na.ssl-images-amazon.com/images/I/81PRr0RBnTL._SL1500_.jpg'
            }
          ]
        },
        {
          userName: 'Kristopher Fager',
          profilePic: 'https://i.imgur.com/RM2ln57.jpg',
          newMessages: {
                          sender: 'notMe',
                          message: 'send noobs',
                          time: '10:35',
                          img: null
                        },
          chatHistory: [
            {
              sender: 'notMe',
              message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime mollitia, molestiae quas vel sint commodi',
              time: '10:35',
              img: null
            },
            {
              sender: 'Me',
              message: 'Lorem ipsum',
              time: '10:37',
              img: 'https://thefanmetareader.files.wordpress.com/2015/07/maxresdefault.jpg'
            },
            {
              sender: 'notMe',
              message: 'dolor sit sint commodi',
              time: '10:41',
              img: null
            }
          ]
        },
        {
          userName: 'Laureen Deangelis',
          profilePic: 'https://i.pinimg.com/originals/ae/ec/c2/aeecc22a67dac7987a80ac0724658493.jpg',
          newMessages: null,
          chatHistory: [
            {
              sender: 'notMe',
              message: 'Lorem ipsum dolor',
              time: '10:35',
              img: null
            },
            {
              sender: 'Me',
              message: 'Hello Google',
              time: '10:37',
              img: null
            },
            {
              sender: 'notMe',
              message: 'Hello user!! dolor sit sint commodi',
              time: '10:41',
              img: null
            }
          ]
        },
        {
          userName: 'Winston Lanni',
          profilePic: 'http://thenewcode.com/assets/images/thumbnails/sarah-parmenter.jpeg',
          newMessages: null,
          chatHistory: [
            {
              sender: 'notMe',
              message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime mollitia, molestiae quas vel sint commodi',
              time: '10:35',
              img: null
            },
            {
              sender: 'Me',
              message: 'Lorem ipsum',
              time: '10:37',
              img: null
            },
            {
              sender: 'notMe',
              message: 'dolor sit sint commodi',
              time: '10:41',
              img: 'https://images-na.ssl-images-amazon.com/images/I/81PRr0RBnTL._SL1500_.jpg'
            }
          ]
        }
      ],
      isMobileDevice: false,
      activeTab: 'Home'
    }
  },
  mounted () {
    const device = navigator.userAgent.toLowerCase()
    const isAndroid = device.includes('android')
    if (isAndroid || !!navigator.platform && /iPad|iPhone|iPod/.test(navigator.platform)) {
      // if user have mobile device (android/ios) then user will only be able to see 7 month graph instead of 12, this could have done with responsive classes also but I was iterating the graph bars with for loop
      // so it was quite tricky to apply responsive sudo classes so I had to figure out a diff method 
      this.graphs = this.graphs.slice(5, 12)
      this.isMobileDevice = true
    } else {
      console.log('big screen device')
    }
    this.previewChat = {...this.ChatJson[0]} // first chat opens up on its own
  },
  methods: {
    sendMessage ($event) { // on pressing enter, we can send message (only on frontend though)
      if (this.writtenMessage.length > 0 && $event.keyCode === 13) {
        const dateObj = new Date()
        const seconds = dateObj.getTime()
        const time = new Date(seconds).toString().slice(16, 21) // got the time of sending message
        const chatObj = {
          sender: 'Me',
          message: this.writtenMessage,
          time,
          img: null
        }
        this.previewChat.chatHistory.push(chatObj) // push new message to existing chunk
        this.writtenMessage = '' // clear the input field
      }
    },
    OpenConversation () {
      this.activeTab = 'Convo'
    },
    OpenChat (idy) {
      this.previewChat = {...this.ChatJson[idy]} // opened the clicked chat
    }
  }
}
</script>

<style>
.chatBoxHeight {
  min-height: 98vh;
}
.line-center{
    margin:0;padding:0 10px;
    background:#fff;
    display:inline-block;
}
.CustomMinimumH {
  min-height: calc(100vh - 5rem);
}
h2:after{
    content:"";
    position:absolute;
    top:50%;
    left:0;
    right:0;
    border-top:solid 1px rgb(136, 130, 130);
    z-index:-1;
}
</style>
