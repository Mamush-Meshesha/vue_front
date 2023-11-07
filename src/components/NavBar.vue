<script setup>
import { RouterLink } from "vue-router";
import { Icon } from "@iconify/vue";
</script>
<template>
  <div>
    <header class="flex w-[1660px] justify-between mx-auto my-10">
      <div>
        <RouterLink to="/" class="text-2xl mx-3 capitalize font-bold"
          >Piche</RouterLink
        >
        <div class="flex text-2xl font-bold w-[90px]">
          <Icon icon="radix-icons:dot-filled" />
          <Icon icon="bi:dot" />
          <Icon icon="ph:dot-bold" />
          <Icon icon="ph:dot" />
          <Icon icon="ph:dot-thin" />
        </div>
      </div>
      <div>
        <RouterLink to="/" class="text-xl mx-3">Home</RouterLink>
        <RouterLink to="/" class="text-xl mx-3">Services</RouterLink>
        <RouterLink to="/" class="text-xl mx-3">Center</RouterLink>
        <RouterLink to="/" class="text-xl mx-3">Work</RouterLink>
        <RouterLink to="/" class="text-xl mx-3">About</RouterLink>
        <RouterLink to="/" class="text-xl mx-3">Contact</RouterLink>
        <button
          to="/"
          class="text-xl mx-3 border-2 rounded-l-full rounded-r-full h-9 w-[120px]"
        >
          Request
        </button>
      </div>
    </header>
  </div>
</template>
