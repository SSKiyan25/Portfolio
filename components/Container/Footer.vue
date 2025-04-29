<template>
  <UiContainer as="footer" class="py-4 lg:py-8">
    <section
      class="flex flex-col items-center justify-between gap-5 pt-8 text-center lg:flex-row lg:text-left"
    >
      <!-- Copyright Text -->
      <p class="text-sm text-muted-foreground sm:text-base">
        &copy; Copyright {{ new Date().getFullYear() }}. Made by Joshua Sosmeña. All rights
        reserved.
      </p>

      <!-- Social Media Icons -->
      <div class="flex flex-wrap items-center justify-center gap-4">
        <UiButton variant="ghost" size="icon-sm">
          <img
            src="/facebook.svg"
            alt="Facebook"
            class="h-6 w-6 opacity-60 hover:opacity-100 sm:h-8 sm:w-8 lg:h-10 lg:w-10"
          />
        </UiButton>
        <UiButton variant="ghost" size="icon-sm">
          <img
            src="/github.svg"
            alt="GitHub"
            class="h-6 w-6 opacity-60 hover:opacity-100 sm:h-8 sm:w-8 lg:h-10 lg:w-10"
          />
        </UiButton>
        <UiButton variant="ghost" size="icon-sm">
          <img
            src="/instagram.svg"
            alt="Instagram"
            class="h-6 w-6 opacity-60 hover:opacity-100 sm:h-8 sm:w-8 lg:h-10 lg:w-10"
          />
        </UiButton>
        <UiButton variant="ghost" size="icon-sm">
          <img
            src="/linkedin.svg"
            alt="LinkedIn"
            class="h-6 w-6 opacity-60 hover:opacity-100 sm:h-8 sm:w-8 lg:h-10 lg:w-10"
          />
        </UiButton>
      </div>
    </section>
  </UiContainer>
</template>
