<template>
  <div class="slidev-layout default-with-footer">
    <div class="my-auto w-full">
      <slot />

      <div class="w-11/12 fixed bottom-0 flex justify-between mb-2 text-sm footer">
        <span>{{ $slidev.configs.shortTitle }} </span>
        <span>{{ $slidev.configs.occasion }} - {{ $slidev.configs.contact }} - {{ $slidev.configs.company }}</span>
        <span style="min-width: 4rem;"><SlideCurrentNo /> / <SlidesTotal /></span>
        </div>
    </div>
  </div>
</template>
