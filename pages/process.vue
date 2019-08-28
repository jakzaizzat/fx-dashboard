<template>
  <div class="dashboard">
    <div class="card">
      <h1>
        Analysis
        <span>Last Month</span>
      </h1>

      <div class="flex flex-wrap">
        <div class="w-1/2 dashboard__card">
          <span>99%</span>
          <div>
            <p>Uptime</p>
          </div>
        </div>
        <div class="w-1/2 dashboard__card">
          <span>2</span>
          <div>
            <p>Process</p>
            <p>Running</p>
          </div>
        </div>
      </div>
    </div>

    <TableCron/>
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
  @apply mb-3 flex items-center p-4 border-r border-grey-light;
}

.dashboard__card:last-child {
  @apply border-none;
}

.dashboard__card span {
  @apply text-4xl text-black pr-4;
}

.dashboard__card p {
  @apply mb-0 font-light text-sm text-grey;
}

.card {
  @apply p-4 bg-white rounded border border-grey-light mb-3;
}
</style>
