<template>
  <div class="h-[100vh] flex justify-center items-center">
    <div class="flex flex-col items-center gap-5">
      <div class="w-40 h-40">
        <img class="rounded-full w-full drop-shadow-xl" src="..\assets\images\picture.PNG" alt="Profile Picture">
      </div>
      <div class="text-center">
        <h1 class="text-3xl font-semibold mb-1">Abulkosim</h1>
        <h3 class="text-xl">Front-end Engineer, CS @ INHA</h3>
      </div>
      <div class="icons flex gap-4">
        <a href="http://github.com/Abulkosim" title="GitHub">
          <PhGithubLogo :size="36" weight="fill" />
        </a>
        <a href="https://www.linkedin.com/in/abulkosim" title="LinkedIn">
          <PhLinkedinLogo :size="36" weight="fill" />
        </a>
        <a href="#" title="CV">
          <PhReadCvLogo :size="36" weight="fill" />
        </a>
        <a href="mailto:abulkasimkattaev@gmail.com" title="Email">
          <PhEnvelopeSimple :size="36" weight="fill" />
        </a>
        <a href="https://t.me/abulkosimkataev" title="Telegram">
          <PhTelegramLogo :size="36" weight="fill" />
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
import { PhTwitterLogo, PhGithubLogo, PhLinkedinLogo, PhTelegramLogo, PhEnvelopeSimple, PhReadCvLogo } from "@phosphor-icons/vue";

</script>

<style scoped>
div {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #333;
}

div a {
  --tw-drop-shadow: drop-shadow(0 20px 13px rgb(0 0 0 / 0.03)) drop-shadow(0 8px 5px rgb(0 0 0 / 0.08));
  filter: var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);
}

.icons a {
  @apply transition-all ease-linear duration-300;
}

.icons a:hover {
  @apply translate-y-[-5px];
}
</style>