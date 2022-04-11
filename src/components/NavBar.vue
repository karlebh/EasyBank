<template>
    <button @click="close" id="close" class="fixed z-20 w-full h-full inset-0 navbar cursor-default">
      <div class="bg-white w-10/12 pt-9 pb-7 mx-auto -mt-56 rounded-lg">
        <a class="block text-center font-semibold" href="#">Home</a>
        <a class="block text-center mt-5 font-semibold" href="#">About</a>
        <a class="block text-center mt-5 font-semibold" href="#">Contact</a>
        <a class="block text-center mt-5 font-semibold" href="#">Blog</a>
        <a class="block text-center mt-5 font-semibold" href="#">Careers</a>
      </div>
    </button>
</template>

<script>
  export default {
    methods: {
      close($event) {
        $event.target.id == 'close' && this.$emit('closeNav')
      }
    }
  }
</script>

<style scoped>
  .navbar {
     background-image: linear-gradient(to bottom, transparent, rgba(0,0,0,0.6));
  }  
</style>