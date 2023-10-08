<template>
  <div class="navbar sticky top-0">
    <div class="flex justify-between py-3 bg-white">
      <div class="cursor-pointer">
        <div class="space-y-2 pt-2" @click="openMenu">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="28"
            height="32"
            viewBox="0 0 448 512"
          >
            <path
              fill="currentColor"
              d="M16 132h416c8.837 0 16-7.163 16-16V76c0-8.837-7.163-16-16-16H16C7.163 60 0 67.163 0 76v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16z"
            />
          </svg>
        </div>
      </div>
      <div class="text-xl">My Food</div>
      <div class="text-xl">Mail</div>
    </div>

    <div
      :class="`absolute w-1/2 h-full top-0 ${
        isOpenMenu ? 'left-0' : 'left-[-900px]'
      } transition-all duration-500`"
    >
      <ul class="text-3xl cursor-pointer bg-white">
        <li class="p-5" @click="openMenu">Close Menu</li>
        <li class="p-5">Food</li>
        <li class="p-5">About</li>
      </ul>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const isOpenMenu = ref(false);
function openMenu() {
  isOpenMenu.value = !isOpenMenu.value;
}
</script>
