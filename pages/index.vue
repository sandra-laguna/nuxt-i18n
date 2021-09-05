<template>
  <main class="h-screen text-white relative">

    <select v-model="$i18n.locale" class="block mx-auto fixed top-10 inset-x-0 text-black">
      <option v-for="lang in $i18n.locales" :key="lang.code" :value="lang.code">{{ lang.name }}</option>
    </select>

    <div class="h-full flex flex-col justify-center items-center">
      <h1 class="text-9xl">{{ $t("message") }}</h1>

      <nuxt-link :to="localePath('index', 'en')" class="text-xl mt-6 hover:underline">&raquo; Homepage in English &laquo;</nuxt-link>
      <nuxt-link :to="localePath('index', 'es')" class="text-xl mb-2 hover:underline">&raquo; Web en español &laquo; </nuxt-link>

      <nuxt-link :to="localePath('/contact')" class="text-xl my-8 border-b hover:text-green-300 hover:border-green-300">{{ $t("pathToContact") }}</nuxt-link>
    </div>
    
  </main>
</template>

