<template>
  <div class="slidev-layout default-with-footer">
    <div class="my-auto w-full">
      <slot />
    </div>

    <div
      style="width: 100%; background-color: hotpink; position: fixed; bottom: 0"
    >
      <SlideCurrentNo /> / <SlidesTotal /> <br />
      {{ $slidev.configs.occasion }} {{ $slidev.configs.company }}
      {{ $slidev.configs.presenter }} {{ $slidev.configs.contact }}
    </div>
  </div>
</template>
