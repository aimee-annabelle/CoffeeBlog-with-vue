<template>
<!-- fontawesome icons link -->
<link rel="stylesheet" 
        href="https://use.fontawesome.com/releases/v5.2.0/css/all.css" 
        integrity="sha384-hWVjflwFxL6sNzntih27bfxkr27PmbbK/iSvJ+a4+0owXq79v+lsFkW54bOGbiDQ" 
        crossorigin="anonymous">
<!-- end -->

  <nav class="relative flex flex-wrap items-center justify-between px-2 py-3 mb-3">
    <div class="container px-4 mx-auto flex flex-wrap items-center justify-between">
      <div class="w-full relative mr-20 flex justify-between lg:w-auto  px-4 lg:static lg:block lg:justify-start">
        <a class="text-xl font-bold leading-relaxed inline-block mr-4 py-2 whitespace-nowrap  text-gray-700" href="#">
          HotCoffee
        </a>
        <button class="text-gray-500 cursor-pointer text-xl leading-none px-3 py-1 border border-solid border-transparent rounded bg-transparent block lg:hidden outline-none focus:outline-none" type="button" v-on:click="toggleNavbar()">
          <i class="fas fa-bars"></i>
        </button>
      </div>
      <div v-bind:class="{'hidden': !showMenu, 'flex': showMenu}" class="lg:flex lg:flex-grow items-center">
        <div class="pt-2 relative mx-auto text-gray-900">
          <button type="submit" class="absolute top-0 mt-5">
          <svg class="text-gray-600 h-4 w-4 fill-current" xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" id="Capa_1" x="0px" y="0px"
            viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 56.966 56.966;" xml:space="preserve"
            width="512px" height="512px">
            <path
              d="M55.146,51.887L41.588,37.786c3.486-4.144,5.396-9.358,5.396-14.786c0-12.682-10.318-23-23-23s-23,10.318-23,23  s10.318,23,23,23c4.761,0,9.298-1.436,13.177-4.162l13.661,14.208c0.571,0.593,1.339,0.92,2.162,0.92  c0.779,0,1.518-0.297,2.079-0.837C56.255,54.982,56.293,53.08,55.146,51.887z M23.984,6c9.374,0,17,7.626,17,17s-7.626,17-17,17  s-17-7.626-17-17S14.61,6,23.984,6z" />
          </svg>
        </button>
        <input class="bg-white h-10 px-10 pr-10 rounded-lg text-base focus:outline-none"
          type="search" name="search" placeholder="Search...">
      </div>
        <ul class="flex flex-col lg:flex-row list-none ml-auto">
          <li class="nav-item">
            <a class="px-3 py-2 flex items-center text-base leading-snug text-gray-700 hover:opacity-75" href="#pablo">
              Home
            </a>
          </li>
          <li class="nav-item">
            <a class="px-7 py-2 flex items-center text-base leading-snug text-gray-700 hover:opacity-75" href="#pablo">
              Articles
            </a>
          </li>
          <li class="nav-item">
            <a class="px-5 py-2 flex items-center text-lg font-bold leading-snug text-gray-700 hover:opacity-75" href="#pablo">
              <i class="fab fa-instagram text-xl leading-lg text-gray-700 opacity-75"></i>
            </a>
          </li>
          <li class="nav-item">
            <a class="px-5 py-2 flex items-center text-lg font-bold leading-snug text-gray-700 hover:opacity-75" href="#pablo">
              <i class="fab fa-twitter text-xl leading-lg text-gray-700 opacity-75" />
            </a>
          </li>
          <li class="nav-item">
            <a class="px-3 py-2 flex items-center text-lg font-bold leading-snug text-gray-700 hover:opacity-75" href="#pablo">
              <i class="fab fa-linkedin text-xl leading-lg text-gray-700 opacity-75"></i>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "navbar",
  data() {
    return {
      showMenu: false
    }
  },
  methods: {
    toggleNavbar: function(){
      this.showMenu = !this.showMenu;
    }
  }
}
</script>

<style>

</style>
