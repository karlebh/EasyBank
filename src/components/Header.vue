<template>
  <header class="bg-white relative z-20">

    <div class="max-w-6xl mx-auto flex justify-between items-center p-6 xl:px-0 relative lg:static z-30">
      <Logo/>

      <div class="text-gray-400 text-sm hidden lg:block">
        <a class="" href="#">Home</a>
        <a class="ml-8" href="#">About</a>
        <a class="ml-8" href="#">Contact</a>
        <a class="ml-8" href="#">Blog</a>
        <a class="ml-8" href="#">Careers</a>
      </div>

       <div class="hidden lg:block">
        <button style="background-image: linear-gradient(to right, hsl(136, 65%, 51%), hsl(192, 70%, 51%))" class="px-10 py-3 text-gray-50 rounded-full text-sm">Request Invite</button>
      </div>


      <!-- Mobile -->
      <button @click="isOpen = !isOpen" class="lg:hidden">
        <svg v-if="!isOpen" xmlns="http://www.w3.org/2000/svg" width="24" height="11"><g fill="#2D314D" fill-rule="evenodd"><path d="M0 0h24v1H0zM0 5h24v1H0zM0 10h24v1H0z"/></g></svg>
        <svg v-if="isOpen" xmlns="http://www.w3.org/2000/svg" width="18" height="19"><g fill="#2D314D" fill-rule="evenodd"><path d="M.868.661l16.97 16.97-.706.708L.162 1.369z"/><path d="M.161 17.632L17.131.662l.708.706-16.97 16.97z"/></g></svg>
      </button>
    </div>


    
    <NavBar @closeNav="isOpen = false" v-if="isOpen"/>
  </header>
</template>

<script>
  import NavBar from '@/components/NavBar'
  import Logo from '@/components/Logo'
  export default {
    data() {
      return {
        isOpen: false,
      }
    },
    components: {
      NavBar,
      Logo,
    },
  }
</script>

