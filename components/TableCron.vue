<template>
  <div class="table">
    <h1>Process Running</h1>
    <div class="row">
      <div class="w-1/2">
        <span class="text-xs text-grey-dark uppercase tracking-wide">Task</span>
      </div>
      <div class="w-1/4">
        <span class="text-xs text-grey-dark uppercase tracking-wide">Status</span>
      </div>
      <div class="w-1/4">
        <span class="text-xs text-grey-dark uppercase tracking-wide">Last Updated</span>
      </div>
    </div>
    <div class="row">
      <div class="w-1/2">
        <p>Listen to market price</p>
      </div>
      <div class="w-1/4">
        <span class="font-semibold text-green">Running</span>
      </div>
      <div class="w-1/4">
        <span class="text-grey-darker text-base">8 minute ago</span>
      </div>
    </div>
    <div class="row">
      <div class="w-1/2">
        <p>Send Weekly Report</p>
      </div>
      <div class="w-1/4">
        <span class="font-semibold text-green">Running</span>
      </div>
      <div class="w-1/4">
        <span class="text-grey-darker text-base">3 days ago</span>
      </div>
    </div>
    <div class="row">
      <div class="w-1/2">
        <p>Telegram authentication</p>
      </div>
      <div class="w-1/4">
        <span class="font-semibold text-red">Stop</span>
      </div>
      <div class="w-1/4">
        <span class="text-grey-darker text-base">10 minute ago</span>
      </div>
    </div>
  </div>
</template>


<style lang="postcss" scoped>
.table {
  @apply bg-white rounded border border-grey-light mb-3 w-full;
}

.table h1 {
  @apply font-medium text-grey-darkest text-xl p-4;
}

.table .row {
  @apply p-4 flex text-grey-darker items-center border-b border-grey-light;
}
</style>
