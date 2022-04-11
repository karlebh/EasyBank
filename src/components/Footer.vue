<template>
  <footer style="background:  hsl(233, 26%, 24%);" class="py-10">
    <div class="flex flex-col items-center lg:flex-row lg:justify-between lg:items-center max-w-6xl mx-auto px-6 xl:px-0">
<!--  -->
      <div class="lg:w-1/4">
        <LogoWhite/>
        <SocialMediaLinks class="mt-5 lg:mt-10"/>
      </div>

      <!-- Mobile -->
      <div class="mx-auto text-center text-gray-300 mt-5 lg:mt-0 lg:hidden">
        <a class="block" href="#">About Us</a>
        <a class="block mt-2" href="#">Contact</a>
        <a class="block mt-2" href="#">Blog</a>
        <a class="block mt-2" href="#">Careers</a>
        <a class="block mt-2" href="#">Support</a>
        <a class="block mt-2" href="#">Privacy Policy</a>
      </div>

      <!-- Desktop -->
      <div class="mx-auto text-center hidden lg:text-left text-gray-300 mt-5 lg:mt-0 lg:w-1/4 lg:flex lg:justify-between">
        <div>
          <a class="block" href="#">About Us</a>
          <a class="block mt-2" href="#">Contact</a>
          <a class="block mt-2" href="#">Blog</a>
        </div>

        <div>
          <a class="block" href="#">Careers</a>
          <a class="block mt-2" href="#">Support</a>
          <a class="block mt-2" href="#">Privacy Policy</a>
        </div>
      </div>

      <div class="mx-auto text-center mt-5 lg:mt-0 lg:mx-0 lg:text-right lg:w-1/2">
        <button style="background-image: linear-gradient(to right, hsl(136, 65%, 51%), hsl(192, 70%, 51%))" 
        class="px-10 py-3 text-gray-100 rounded-full text-sm">Request Invite</button>
        <p class="mt-4 lg:mt-6 text-gray-400">&copy; Easybank. All rights reserved.</p>
      </div>

    </div>
  </footer>
</template>

<script>
  import LogoWhite from '@/components/LogoWhite'
  import SocialMediaLinks from '@/components/SocialMediaLinks'

  export default {
    components: { 
      LogoWhite,
      SocialMediaLinks,
     }
  }
</script>
