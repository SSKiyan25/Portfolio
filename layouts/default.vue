<template>
  <div class="flex min-h-screen flex-col">
    <header class="sticky top-0 z-40 border-b bg-primary/90 text-primary-foreground backdrop-blur">
      <UiContainer class="flex h-16 items-center justify-between lg:h-20">
        <div class="flex items-center gap-10">
          <NuxtLink to="/" class="flex items-center gap-3">
            <img
              src="/me.jpg"
              alt="Joshua Sosmeña"
              class="h-4 w-4 rounded-full object-cover sm:h-12 sm:w-12 lg:h-14 lg:w-14"
              loading="lazy"
            />
            <span class="font-semibold lg:text-lg">Joshua Sosmeña</span>
          </NuxtLink>
        </div>
        <div class="items-center gap-3">
          <UiNavigationMenu as="nav" class="hidden items-center gap-8 lg:flex">
            <UiNavigationMenuList class="gap-2">
              <UiNavigationMenuItem>
                <UiNavigationMenuLink as-child>
                  <UiButton to="#header" variant="ghost" size="sm"> Home</UiButton>
                </UiNavigationMenuLink>
              </UiNavigationMenuItem>
              <UiNavigationMenuItem>
                <UiNavigationMenuLink as-child>
                  <UiButton to="#about" variant="ghost" size="sm">About</UiButton>
                </UiNavigationMenuLink>
              </UiNavigationMenuItem>
              <UiNavigationMenuItem>
                <UiNavigationMenuLink as-child>
                  <UiButton to="#projects" variant="ghost" size="sm">Projects</UiButton>
                </UiNavigationMenuLink>
              </UiNavigationMenuItem>
              <UiNavigationMenuItem>
                <UiNavigationMenuLink as-child>
                  <UiButton to="#contact" variant="ghost" size="sm">Contact</UiButton>
                </UiNavigationMenuLink>
              </UiNavigationMenuItem>
            </UiNavigationMenuList>
          </UiNavigationMenu>
          <div class="lg:hidden">
            <UiSheet>
              <UiSheetTrigger as-child>
                <UiButton variant="ghost" size="icon-sm">
                  <Icon name="lucide:menu" class="h-5 w-5" />
                </UiButton>
                <UiSheetContent class="w-[90%] p-0">
                  <template #content>
                    <UiSheetTitle class="sr-only" title="Mobile menu" />
                    <UiSheetDescription class="sr-only" description="Mobile menu" />
                    <UiSheetX class="z-20" />

                    <UiScrollArea class="h-full p-5">
                      <div class="flex flex-col gap-2">
                        <UiButton variant="ghost" class="justify-start text-base" to="#header"
                          >Home</UiButton
                        >
                        <UiButton variant="ghost" class="justify-start text-base" to="#about"
                          >About</UiButton
                        >
                        <UiButton variant="ghost" class="justify-start text-base" to="#projects"
                          >Projects</UiButton
                        >
                        <UiButton variant="ghost" class="justify-start text-base" to="#contact"
                          >Contact</UiButton
                        >
                      </div>
                    </UiScrollArea>
                  </template>
                </UiSheetContent>
              </UiSheetTrigger>
            </UiSheet>
          </div>
        </div>
      </UiContainer>
    </header>
    <div class="mt-0 min-h-screen flex-col">
      <slot />
    </div>
  </div>
</template>

<script lang="ts" setup></script>
