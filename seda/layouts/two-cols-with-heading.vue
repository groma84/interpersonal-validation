<template>
  <div class="slidev-layout two-cols-with-heading">
    <div class="my-auto w-full">
      <slot name="heading" />

      <div class="my-auto w-full flex justify-between">

        <div style="flex: 1;">
          <slot name="left" />
        </div>

        <div style="flex: 1; border-left: 1px solid var(--slidev-theme-primary)" class="pl-2">
          <slot name="right" />
        </div>

      </div>

      <div class="w-11/12 fixed bottom-0 flex justify-between mb-2 text-sm footer">
        <span>{{ $slidev.configs.shortTitle }} </span>
        <span>{{ $slidev.configs.company }} - {{ $slidev.configs.speaker }} - {{ $slidev.configs.contact }}</span>
        <span style="min-width: 4rem;"><SlideCurrentNo /> / <SlidesTotal /></span>
        </div>
    </div>
  </div>
</template>
