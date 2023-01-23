
<template>
  <div class="isolate bg-white">
    <div class="absolute inset-x-0 top-[-10rem] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[-20rem]">
      <svg class="relative left-[calc(50%-11rem)] -z-10 h-[21.1875rem] max-w-none -translate-x-1/2 rotate-[30deg] sm:left-[calc(50%-30rem)] sm:h-[42.375rem]" viewBox="0 0 1155 678" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill="url(#45de2b6b-92d5-4d68-a6a0-9b9b2abad533)" fill-opacity=".3" d="M317.219 518.975L203.852 678 0 438.341l317.219 80.634 204.172-286.402c1.307 132.337 45.083 346.658 209.733 145.248C936.936 126.058 882.053-94.234 1031.02 41.331c119.18 108.451 130.68 295.337 121.53 375.223L855 299l21.173 362.054-558.954-142.079z" />
        <defs>
          <linearGradient id="45de2b6b-92d5-4d68-a6a0-9b9b2abad533" x1="1155.49" x2="-78.208" y1=".177" y2="474.645" gradientUnits="userSpaceOnUse">
            <stop stop-color="#9089FC" />
            <stop offset="1" stop-color="#FF80B5" />
          </linearGradient>
        </defs>
      </svg>
    </div>
    <div class="px-6 pt-6 lg:px-8">
      <div>
        <nav class="flex h-9 items-center justify-between" aria-label="Global">
          <!-- <div class="flex lg:min-w-0 lg:flex-1" aria-label="Global">
            Add your profile image
          </div> -->
          <div class="flex lg:hidden">
            <button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700" @click="mobileMenuOpen = true">
              <span class="sr-only">Open main menu</span>
              <Bars3Icon class="h-6 w-6" aria-hidden="true" />
            </button>
          </div>
          <div class="hidden lg:flex lg:min-w-0 lg:flex-1 lg:justify-center lg:gap-x-12">
            <a v-for="item in navigation" :key="item.name" :href="item.href" class="font-semibold text-gray-900 hover:text-gray-900">{{ item.name }}</a>
          </div>
          
        </nav>
        <Dialog as="div" @close="mobileMenuOpen = false" :open="mobileMenuOpen">
          <DialogPanel focus="true" class="fixed inset-0 z-10 overflow-y-auto bg-white px-6 py-6 lg:hidden">
            <div class="flex h-9 items-center justify-between">
              <div class="flex">
                <!-- <a href="#" class="-m-1.5 p-1.5">
                  <span class="sr-only">Your Company</span>
                  <img class="h-8" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600" alt="" />
                </a> -->
              </div>
              <div class="flex">
                <button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700" @click="mobileMenuOpen = false">
                  <span class="sr-only">Close menu</span>
                  <XMarkIcon class="h-6 w-6" aria-hidden="true" />
                </button>
              </div>
            </div>
            <div class="mt-6 flow-root">
              <div class="-my-6 divide-y divide-gray-500/10">
                <div class="space-y-2 py-6">
                  <a v-for="item in navigation" :key="item.name" :href="item.href" class="-mx-3 block rounded-lg py-2 px-3 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-400/10">{{ item.name }}</a>
                </div>
                <div class="py-6">
                  <a href="#" class="-mx-3 block rounded-lg py-2.5 px-3 text-base font-semibold leading-6 text-gray-900 hover:bg-gray-400/10">Log in</a>
                </div>
              </div>
            </div>
          </DialogPanel>
        </Dialog>
      </div>
    </div>
    <main>
      <div class="relative px-6 lg:px-8">
        <div class="mx-auto max-w-3xl pt-20 pb-32 sm:pt-48 sm:pb-40">
          <div>
            <div class="hidden sm:mb-8 sm:flex sm:justify-center">
              <div class="relative overflow-hidden rounded-full py-1.5 px-4 text-sm leading-6 ring-1 ring-gray-900/10 hover:ring-gray-900/20">
                <span class="text-gray-600">
                  Lets Work together  <a href="#" class="font-semibold text-indigo-600"><span class="absolute inset-0" aria-hidden="true" />Contact Me<span aria-hidden="true">&rarr;</span></a>
                </span>
              </div>
            </div>
            <div>
              <h1 class="text-4xl font-bold tracking-tight sm:text-center sm:text-6xl">Hey guys, This is Maimuna Al-Wahaibi!</h1>
              <p class="mt-6 text-lg leading-8 text-gray-600 sm:text-center"><Note>A brief summary about me, I'm an energetic and self-motivated Sultan Qaboos University student with an outstanding
performer in machine learning and web application development. Proven success in
leadership and group work. A leader and active member in the student societies.</Note></p>
              <div class="mt-8 flex gap-x-4 sm:justify-center" >
                <a href="src/assets/CV.pdf" class="inline-block rounded-lg bg-indigo-600 px-4 py-1.5 text-base font-semibold leading-7 text-white shadow-sm ring-1 ring-indigo-600 hover:bg-indigo-700 hover:ring-indigo-700">
                  Download Resume{{ '' }}
                  <span class="text-indigo-200" aria-hidden="true">&rarr;</span>
                  
                </a>
                <br>
                <input v-model="title" type="text" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-100px p-2.5 " placeholder="type to change the title">
  
              </div>
            </div>
            <div class="absolute inset-x-0 top-[calc(100%-13rem)] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[calc(100%-30rem)]">
              <svg class="relative left-[calc(50%+3rem)] h-[21.1875rem] max-w-none -translate-x-1/2 sm:left-[calc(50%+36rem)] sm:h-[42.375rem]" viewBox="0 0 1155 678" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill="url(#ecb5b0c9-546c-4772-8c71-4d3f06d544bc)" fill-opacity=".3" d="M317.219 518.975L203.852 678 0 438.341l317.219 80.634 204.172-286.402c1.307 132.337 45.083 346.658 209.733 145.248C936.936 126.058 882.053-94.234 1031.02 41.331c119.18 108.451 130.68 295.337 121.53 375.223L855 299l21.173 362.054-558.954-142.079z" />
                <defs>
                  <linearGradient id="ecb5b0c9-546c-4772-8c71-4d3f06d544bc" x1="1155.49" x2="-78.208" y1=".177" y2="474.645" gradientUnits="userSpaceOnUse">
                    <stop stop-color="#9089FC" />
                    <stop offset="1" stop-color="#FF80B5" />
                  </linearGradient>
                </defs>
              </svg>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>



 
  <div id="app" class="bg-slate-50 w-50">
  <div class="flex">
  
  <div class="  p-6  border border-gray-200 rounded-lg shadow-md hover:bg-gray-100 card inline-block w-1/2 mr-4 bg-gray-200">
  <note>Text
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</note>
  </div><br>
  <div class=" p-6  border border-gray-200 rounded-lg shadow-md hover:bg-gray-100 card inline-block w-1/2 bg-gray-200">
    <note>Selected Text</note><br>
  <p>{{state.text}}</p>
  </div>
    </div>
    <br>
    
   
  </div> 
</template>





<script setup lang="ts">

// import { Dialog, DialogPanel } from '@headlessui/vue'
// import { Bars3Icon, XMarkIcon } from '@heroicons/vue/24/outline'
import { useTextSelection } from '@vueuse/core'
import { useTitle } from '@vueuse/core'
import { useWindowFocus } from '@vueuse/core'
import { ref, watch } from 'vue'

const navigation = [
  { name: 'About Me', href: '#' },
  { name: 'Skills', href: '#pages/skills.vue' },
  { name: 'Projects', href: '#' },
  { name: 'Contact', href: '#' },
]

const mobileMenuOpen = ref(false)
const state = useTextSelection()


const startMessage = 'Try me out 🥰 '
const message = ref(startMessage)
const title = useTitle(startMessage)
const focused = useWindowFocus()


watch(focused, (isFocused) => {
  if (isFocused){
    message.value = startMessage
    useTitle(message.value)
  }
  else
    message.value = '👀Come back'
    useTitle(message.value)
}

)



</script>

<style scoped>
html, body, h1, h2, h3, p {
  font-family: 'Noto Serif', serif;
  user-select: none;
}

#app {
  
  text-align: center;

  color: rgb(20, 20, 20);
}
img {
  width: 500px;
}
a {
  color: #41b883;
  text-decoration: none;
  cursor: pointer;
}



</style>
