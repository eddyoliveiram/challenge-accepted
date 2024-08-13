<template>
  <div class="navbar bg-primary">
    <div class="navbar-start">
      <div ref="dropdown" class="dropdown relative">
        <div tabindex="0" role="button" class="btn btn-ghost md:hidden flex items-center space-x-2" @click.stop="toggleDropdown">
          <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6 btn-primary"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor">
            <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h8m-8 6h16" />
          </svg>
          <span class="text-lg btn-primary">Menu</span>
        </div>
        <ul
            tabindex="0"
            class="menu menu-sm dropdown-content bg-base-100 rounded-box z-[1] mt-3 w-64 p-4 shadow-lg text-xl absolute">
          <li><a href="/" class="h-16 flex items-center">Login</a></li>
          <li>
            <details>
              <summary class="h-16 flex items-center">Parent</summary>
              <ul class="p-2 pl-4">
                <li><a class="h-12 flex items-center">Submenu 1</a></li>
                <li><a class="h-12 flex items-center">Submenu 2</a></li>
              </ul>
            </details>
          </li>
          <li><a href="/about" class="h-16 flex items-center">About</a></li>
        </ul>
      </div>
    </div>
    <div class="navbar-center hidden md:flex">
      <ul class="menu menu-horizontal px-1">
        <li><a href="/" class="btn-primary text-base">Login</a></li>
        <li>
          <details>
            <summary class="btn-primary text-base">Parent</summary>
            <ul class="p-2 w-48">
              <li><a>Submenu 1</a></li>
              <li><a>Submenu 2</a></li>
            </ul>
          </details>
        </li>
        <li><a href="/about" class="btn-primary text-base">About</a></li>
      </ul>
    </div>
    <div class="navbar-end">
      <a href="/logout" class="btn btn-primary">Logout</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavbarStructure',
};
</script>


<style scoped>
</style>
