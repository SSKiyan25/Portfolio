<template>
  <div class="bg-secondary px-6 py-4 sm:px-12 sm:py-8 lg:px-20 lg:py-12">
    <!-- About Me Section -->
    <div class="flex flex-col items-center justify-center p-4 sm:p-8">
      <h2
        class="border-b-4 border-primary/90 text-2xl font-semibold uppercase tracking-wider sm:text-3xl lg:text-4xl"
      >
        About Me
      </h2>
      <p class="pt-4 text-center text-base tracking-wider sm:pt-6 sm:text-lg lg:text-xl">
        Hi! I'm Joshua Sosmeña, Nice to meet you!
      </p>
    </div>

    <!-- Main Content Section -->
    <div class="flex flex-col gap-12 lg:flex-row lg:gap-24">
      <!-- Get to Know Me Section -->
      <div class="flex flex-col space-y-4 lg:w-1/2">
        <h3 class="text-lg font-semibold sm:text-xl lg:text-2xl">Get to know me!</h3>
        <p class="lg:text-md text-justify text-sm leading-6 sm:text-base sm:leading-7 lg:leading-8">
          I'm a <strong>Full-Stack Web Developer</strong> currently pursuing a Bachelor of Science
          in Computer Science (BSCS-3) at Visayas State University.
          <br />
          Beyond coding, I am also a leader, having served as the President of the Computer Science
          Students Society for the school year 2023-2024 and now serving as the Secretary for
          2024-2025. <br />
          I am passionate about building and managing web applications that contribute to the
          success of the overall product. Additionally, I have been a youth volunteer with the
          Claretian Youth Ministry since 2012, where I actively contribute to community-building
          initiatives. <br />
          Feel free to connect with me on Facebook, Github, LinkedIn, or Instagram. I'm open to job
          opportunities where I can contribute, learn, and grow. If you have an opportunity that
          aligns with my skills and experience, don't hesitate to reach out!
        </p>
      </div>

      <!-- My Skills Section -->
      <div class="flex flex-col space-y-4 lg:w-1/2">
        <h3 class="text-lg font-semibold sm:text-xl lg:text-2xl">My Skills</h3>
        <div v-for="(skills, category) in categorizedSkills" :key="category" class="mb-4">
          <!-- Category Title -->
          <h4 class="sm:text-md text-base font-medium lg:text-lg">{{ category }}</h4>
          <!-- Skills List -->
          <div class="flex flex-row flex-wrap gap-2">
            <div
              v-for="skill in skills"
              :key="skill"
              class="lg:text-md rounded-md bg-black/20 p-2 text-sm sm:text-base"
            >
              {{ skill }}
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
  const categorizedSkills = {
    "Programming Languages": ["C", "C++", "Java", "JavaScript", "TypeScript", "PHP"],
    "Libraries and Frameworks": [
      "Vue",
      "Nuxt.js",
      "EJS",
      "Node.js",
      "Express.js",
      "Tailwind CSS",
      "Flutter",
    ],
    Databases: ["Firestore Firebase", "MySQL"],
    "Tools and Platforms": [
      "Git",
      "GitHub",
      "Vercel",
      "Figma",
      "Firebase",
      "Visual Studio Code",
      "Wordpress",
    ],
  };
</script>
