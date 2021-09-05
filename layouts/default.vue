<template>
  <div class="relative w-full h-full  overflow-hidden">

    <app-main>
      <transition mode="out-in">
        <nuxt :key="$route.fullPath" />
      </transition>
    </app-main>

  </div>
</template>
