<template>
  <div class="h-screen">
    <Header class="flex w-full h-[50px]" />
    <div class="flex h-full">
      <Navigation class="flex w-[150px]" />
      <div class="flex-1 p-4">
        <NuxtPage />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
  // プラグインで実装した処理を呼び出し (プログラムから)
  const nuxtApp = useNuxtApp();
  console.log(nuxtApp.$appUrl.siteUrl());
</script>
