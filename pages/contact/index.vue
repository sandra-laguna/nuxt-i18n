<template>
<div class="h-screen text-white"> 
  <div class="h-full flex flex-col justify-center items-center"> 
    <h1 class="font-black text-5xl">{{ $t("contact") }}</h1>

    <nuxt-link :to="localePath('/')" class="bg-green-500 hover:bg-green-700 text-white font-bold py-2 px-4 rounded mt-10">
        {{ $t("btnReturn") }}
    </nuxt-link>
  </div>
</div>
</template>

<script>
export default {
  head() {
    return {
      title: "Contacto | Template",
      link: [{ rel: "canonical", hid: "canonical", href: `${this.$config.baseUrl}/contacto` }]
    };
  }
};
</script>
