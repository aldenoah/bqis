<template>
  <section>
    <nav class="bg-black px-6 py-4">
  <div class="flex items-center justify-between flex-wrap mx-auto">
    <a href="/" class="flex items-center flex-no-shrink text-yellow-dark mr-6 no-underline">
      <span class="font-semibold text-2xl text-shadow tracking-tight">Balqis</span>
    </a>
    <div class="flex items-center w-auto ml-auto">
      <div class="text-sm flex-grow">
        <a href="/" class="hidden md:inline-block mt-0 inline-block text-white hover:text-yellow mr-4 no-underline">Home</a>
        <a href="https://goo.gl/maps/ijXnYxtqKvC2" target="_blank" class="hidden md:inline-block mt-0 inline-block text-white hover:text-yellow mr-4 no-underline">View On Map</a>
        <a href="/contact" class="hidden md:inline-block mt-0 inline-block text-white hover:text-yellow no-underline">Contact Us</a>
      </div>
    </div>
    <div>
      <button class="flex items-center md:hidden px-3 py-2 border text-white border-white hover:text-yellow hover:border-yellow" @click="menu = !menu"> <!-- v-on-clickaway="closeMenu" -->
        <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
      </button>
    </div>
  </div>
</nav>
<ul class="text-center bg-black list-reset py-2" v-show="menu">
  <li class="py-2"><a href="/" class="md:inline-block mt-0 inline-block text-white hover:text-yellow no-underline">Home</a></li>
  <li class="py-2"><a href="https://goo.gl/maps/ijXnYxtqKvC2" target="_blank" class="md:inline-block mt-0 inline-block text-white hover:text-yellow no-underline">View On Map</a></li>
  <li class="py-2"><a href="/contact" class="md:inline-block mt-0 inline-block text-white hover:text-yellow no-underline">Contact</a></li>
</ul>
  </section>
</template>

<script>
  export default {
    data: function() {
      return {
        menu: false
      }
    },
    methods: {
      closeMenu: function() {
        this.menu = false
      }
    }
  }
</script>