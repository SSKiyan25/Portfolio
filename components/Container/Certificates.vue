<template>
  <div class="bg-secondary px-6 py-4 sm:px-12 sm:py-8 lg:px-20 lg:py-12">
    <!-- Certificates Section -->
    <div class="flex flex-col items-center justify-center p-4 sm:p-8">
      <h2
        class="border-b-4 border-primary/90 text-2xl font-semibold uppercase tracking-wider sm:text-3xl lg:text-4xl"
      >
        Certificates
      </h2>
      <p class="pt-4 text-base tracking-wider sm:pt-6 sm:text-lg lg:text-xl">
        Here are some of the certificates I have earned.
      </p>
    </div>

    <!-- Certificates Content -->
    <div class="flex w-full flex-col justify-center gap-12 pt-8 sm:flex-row">
      <!-- Certificate 1 -->
      <div class="flex w-full flex-col items-center space-y-4 px-4 sm:w-1/2 lg:w-1/2">
        <img
          src="/qnlp.png"
          alt="Certificate 1"
          class="h-auto w-full max-w-md rounded-md border object-cover shadow-md"
        />
        <h3 class="sm:text-md text-center text-xs font-semibold lg:text-lg">
          QCSP Lecture Series: Introduction to Quantum <br />
          Natural Language Processing
        </h3>
        <p class="lg:text-md/8 text-justify text-xs/8 sm:text-sm/8">
          Awarded by the Quantum Computing Society of the Philippines in recognition of active
          participation in the QCSP Lecture Series: Introduction to Quantum Natural Language
          Processing, held from September 7, 2024, to November 30, 2024. This event was organized by
          the Quantum Computing Society of the Philippines and its partners.
        </p>
      </div>

      <!-- Certificate 2 -->
      <div class="flex w-full flex-col items-center space-y-4 px-4 sm:w-1/2 lg:w-1/2">
        <img
          src="/claret.png"
          alt="Certificate 2"
          class="h-auto w-full max-w-md rounded-md border object-cover shadow-md"
        />
        <h3 class="sm:text-md text-center text-xs font-semibold lg:text-lg">
          Certificate of Completion: Basic Web Design <br />
          and WordPress Workshop
        </h3>
        <p class="lg:text-md/8 text-justify text-xs/8 sm:text-sm/8">
          Awarded by iClaret Missionari Clarettiani - Curia Generalizia, Via del Sacro Cuore di
          Maria, 5 Roma, Italia, for completing the online workshop on Basic Web Design, WordPress
          Web Creation, and the Use of Social Media held from February 6-10, 2023.
        </p>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style></style>
