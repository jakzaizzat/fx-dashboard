<template>
  <div class="table">
    <h1>Market Open</h1>
    <div class="row">
      <div class="w-1/4">
        <span class="text-xs text-grey-dark uppercase tracking-wide">Currency</span>
      </div>
      <div class="w-1/4">
        <span class="text-xs text-grey-dark uppercase tracking-wide">Open Price</span>
      </div>
      <div class="w-1/4">
        <span class="text-xs text-grey-dark uppercase tracking-wide">Take Profit</span>
      </div>
      <div class="w-1/4">
        <span class="text-xs text-grey-dark uppercase tracking-wide">Stop Loss</span>
      </div>
    </div>
    <div class="row">
      <div class="w-1/4">
        <p>GBPAUD</p>
        <span class="text-xs font-light">3 Days ago</span>
      </div>
      <div class="w-1/4">
        <p class="text-sm text-blue font-bold">BUY</p>
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
      <div class="w-1/4">
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
      <div class="w-1/4">
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
    </div>
    <div class="row">
      <div class="w-1/4">
        <p>GBPAUD</p>
        <span class="text-xs font-light">3 Days ago</span>
      </div>
      <div class="w-1/4">
        <p class="text-sm text-blue font-bold">BUY</p>
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
      <div class="w-1/4">
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
      <div class="w-1/4">
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
    </div>
    <div class="row">
      <div class="w-1/4">
        <p>GBPAUD</p>
        <span class="text-xs font-light">3 Days ago</span>
      </div>
      <div class="w-1/4">
        <p class="text-sm text-blue font-bold">BUY</p>
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
      <div class="w-1/4">
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
      <div class="w-1/4">
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
    </div>
    <div class="row">
      <div class="w-1/4">
        <p>GBPAUD</p>
        <span class="text-xs font-light">3 Days ago</span>
      </div>
      <div class="w-1/4">
        <p class="text-sm text-blue font-bold">BUY</p>
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
      <div class="w-1/4">
        <span class="font-bold text-grey-darker">1.8102</span>
      </div>
      <div class="w-1/4">
        <span class="font-bold text-grey-darker">1.8102</span>
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

.row p {
  @apply tracking-wide;
}
</style>
