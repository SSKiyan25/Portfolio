<script setup lang="ts">
  useHead({
    title: "Joshua Sosmeña | Web Developer",
    link: [
      {
        rel: "icon",
        type: "image/jpg",
        href: "/icon.jpg",
      },
    ],
    meta: [
      { property: "og:title", content: "Joshua Sosmeña | Web Developer" },
      {
        property: "og:description",
        content: "Aspiring Software Engineer, currently studying as BSCS in VSU-Baybay",
      },
      { property: "og:image", content: "https://joshua-sosmena-portfolio.vercel.app/icon.jpg?v=1" },
      { property: "og:url", content: "https://joshua-sosmena-portfolio.vercel.app/" },
      { property: "og:type", content: "website" },

      { name: "twitter:card", content: "summary_large_image" },
      { name: "twitter:title", content: "Joshua Sosmeña | Web Developer" },
      {
        name: "twitter:description",
        content: "Aspiring Software Engineer, currently studying as BSCS in VSU-Baybay",
      },
      { name: "twitter:image", content: "https://joshua-sosmena-portfolio.vercel.app/icon.jpg" },
    ],
  });
</script>
<template>
  <NuxtLoadingIndicator />
  <NuxtLayout>
    <NuxtPage />
    <UiVueSonner />
    <UiToastToaster />
  </NuxtLayout>
</template>
