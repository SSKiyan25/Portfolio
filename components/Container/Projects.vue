<template>
  <UiContainer>
    <!-- Projects Section -->
    <div class="flex flex-col items-center justify-center p-4 sm:p-8">
      <h2
        class="border-b-4 border-primary/90 text-2xl font-semibold uppercase tracking-wider sm:text-3xl lg:text-4xl"
      >
        Projects
      </h2>
      <p class="pt-4 text-center text-base tracking-wider sm:pt-6 sm:text-lg lg:text-xl">
        Here are some of my projects that I have worked on. Feel free to explore them!
      </p>
      <div class="flex w-full flex-col space-y-12 pt-8">
        <!-- Verch Project -->
        <div class="flex flex-col justify-between gap-6 lg:flex-row">
          <div
            class="flex w-full justify-center overflow-hidden rounded-md bg-secondary-foreground/20 p-4 sm:p-8 lg:w-1/2"
          >
            <img
              src="/verch.png"
              alt="Verch"
              class="h-auto w-full max-w-md transform rounded-md border object-cover shadow-md transition-transform duration-300 ease-in-out hover:scale-110"
            />
          </div>
          <div class="flex w-full flex-col space-y-4 px-4 sm:px-8 lg:w-1/2 lg:px-12">
            <h3 class="text-center text-lg font-semibold sm:text-xl lg:text-2xl">Verch</h3>
            <p class="py-2 text-justify text-sm leading-6 sm:text-base lg:text-lg">
              Developed and managed an e-commerce platform for Visayas State University Baybay
              organizations, enabling centralized sales for VSU students. Key features include
              product listings, add-to-cart functionality, and a user-friendly interface. Built with
              Vue.js, NuxtJS, and Firebase, and deployed on Vercel for real-time performance.
            </p>
          </div>
        </div>

        <!-- Soundboard Project -->
        <div class="flex flex-col justify-between gap-6 lg:flex-row">
          <div
            class="flex h-96 w-full justify-center overflow-hidden rounded-md bg-secondary-foreground/20 p-4 sm:p-8 lg:w-1/2"
          >
            <img
              src="/soundboard.jpg"
              alt="Soundboard"
              class="h-auto w-full max-w-md transform rounded-md border object-cover shadow-md transition-transform duration-300 ease-in-out hover:scale-110"
            />
          </div>
          <div class="flex w-full flex-col space-y-4 px-4 sm:px-8 lg:w-1/2 lg:px-12">
            <h3 class="text-center text-lg font-semibold sm:text-xl lg:text-2xl">Soundboard</h3>
            <p class="py-2 text-justify text-sm leading-6 sm:text-base lg:text-lg">
              Created and launched a mobile application with core features including play, pause,
              skip, and search for locally stored songs, all accessible offline. Developed within
              two weeks using Flutter as the cross-platform framework, showcasing its usability and
              efficiency for mobile app development.
            </p>
          </div>
        </div>

        <!-- Weather Classification Project -->
        <div class="flex flex-col justify-between gap-6 lg:flex-row">
          <div
            class="flex w-full justify-center overflow-hidden rounded-md bg-secondary-foreground/20 p-4 sm:p-8 lg:w-1/2"
          >
            <img
              src="/weather.png"
              alt="Weather Classification"
              class="h-auto w-full max-w-md transform rounded-md border object-cover shadow-md transition-transform duration-300 ease-in-out hover:scale-110"
            />
          </div>
          <div class="flex w-full flex-col space-y-4 px-4 sm:px-8 lg:w-1/2 lg:px-12">
            <h3 class="text-center text-lg font-semibold sm:text-xl lg:text-2xl">
              Weather Classification
            </h3>
            <p class="py-2 text-justify text-sm leading-6 sm:text-base lg:text-lg">
              Built a MobileNetV2-based classifier to identify weather conditions (sunny, cloudy,
              rainy), achieving 97% validation accuracy despite a small, imbalanced dataset of 766
              images. Designed a custom head with Global Pooling, Dropout, and Dense layers to
              prevent overfitting, and proposed scalability improvements such as data augmentation
              and ensembling.
            </p>
          </div>
        </div>
      </div>
    </div>
  </UiContainer>
</template>

<script lang="ts" setup></script>

<style></style>
