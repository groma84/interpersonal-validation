<template>
  <div class="slidev-layout cover">
    <div class="flex flex-col justify-between items-start ml-5">
      <img src="/logos/semikron-danfoss.svg" alt="Semikron Danfoss Logo" class="w-50 object-fit-contain" />

      <div class="flex flex-col justify-center items-start ml-5 mt-10">
        <slot />
      </div>

      <div class="w-full flex justify-center">
        <img v-if="!!$slidev.configs.occasionLogoUrl" :src="$slidev.configs.occasionLogoUrl" alt="Occasion Logo" class="w-20 object-fit-contain" />
      </div>
    </div>
  </div>
</template>
