<template>
  <UiContainer>
    <div
      class="flex flex-col items-center justify-center space-y-8 px-4 py-10 sm:px-8 sm:py-16 lg:px-16 lg:py-20"
    >
      <!-- Title -->
      <div class="space-y-2">
        <h1 class="text-center text-xl font-bold uppercase tracking-widest sm:text-3xl lg:text-4xl">
          Full-Stack Developer
        </h1>
        <UiGradientDivider />
      </div>

      <!-- Description -->
      <p class="mt-2 text-center font-mono text-sm opacity-80 sm:text-lg lg:text-xl">
        I am passionate about coding and creating simple solutions. I enjoy learning new
        technologies and continuously improving my craft.
      </p>

      <!-- Profile Image -->
      <div class="pt-4">
        <img
          src="/icon.jpg"
          alt="Joshua Sosmeña"
          class="h-40 w-40 rounded-full object-cover sm:h-48 sm:w-48 lg:h-60 lg:w-60"
          loading="lazy"
        />
      </div>

      <!-- Social Media Buttons -->
      <div class="flex flex-row space-x-4 pt-4">
        <UiButton to="#" variant="ghost" size="sm">
          <img
            src="/facebook.svg"
            alt="Facebook"
            class="h-8 w-8 opacity-60 hover:opacity-100 sm:h-10 sm:w-10"
          />
        </UiButton>
        <UiButton to="#" variant="ghost" size="sm">
          <img
            src="/github.svg"
            alt="GitHub"
            class="h-8 w-8 opacity-60 hover:opacity-100 sm:h-10 sm:w-10"
          />
        </UiButton>
        <UiButton to="#" variant="ghost" size="sm">
          <img
            src="/instagram.svg"
            alt="Instagram"
            class="h-8 w-8 opacity-60 hover:opacity-100 sm:h-10 sm:w-10"
          />
        </UiButton>
        <UiButton to="#" variant="ghost" size="sm">
          <img
            src="/linkedin.svg"
            alt="LinkedIn"
            class="h-8 w-8 opacity-60 hover:opacity-100 sm:h-10 sm:w-10"
          />
        </UiButton>
      </div>
    </div>
  </UiContainer>
</template>

<script lang="ts" setup></script>

<style></style>
