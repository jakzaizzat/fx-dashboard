<template>
  <div class="dashboard">
    <div class="card">
      <h1>
        Analysis
        <span>Last Month</span>
      </h1>

      <div class="flex flex-wrap">
        <div class="w-full md:w-1/2 dashboard__card">
          <span>EUR/USD</span>
          <div>
            <p class="text-green">+ 1320 PIPS</p>
          </div>
        </div>
        <div class="w-full md:w-1/2 dashboard__card">
          <span>GBPJPY</span>
          <div>
            <p class="text-red">-129 PIPS</p>
          </div>
        </div>
      </div>
    </div>
    <div class="card">
      <h1>
        Analysis
        <span>Last Week</span>
      </h1>

      <div class="flex flex-wrap">
        <div class="w-full md:w-1/2 dashboard__card">
          <span>EUR/USD</span>
          <div>
            <p class="text-green">+ 130 PIPS</p>
          </div>
        </div>
        <div class="w-full md:w-1/2 dashboard__card">
          <span>GBPJPY</span>
          <div>
            <p class="text-red">-40 PIPS</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TableCron from "@/components/TableCron";
export default {
  components: {
    TableCron
  }
};
</script>



<style lang="postcss" scoped>
.dashboard {
  @apply p-4;
}

.dashboard h1 {
  @apply font-medium text-grey-darkest text-xl mb-4;
}

.dashboard h1 span {
  @apply text-sm font-normal;
}

.dashboard__card {
  @apply mb-3 flex flex-col items-center justify-center p-4 border-r border-grey-light;
}

.dashboard__card:last-child {
  @apply border-none;
}

.dashboard__card span {
  @apply text-2xl font-bold text-black tracking-wide mb-2;
}

.dashboard__card p {
  @apply mb-0 text-base;
}

.card {
  @apply p-4 bg-white rounded border border-grey-light mb-3;
}
</style>
