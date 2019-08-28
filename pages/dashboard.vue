<template>
  <div class="dashboard">
    <div class="card">
      <h1>
        Analysis
        <span>Last Month</span>
      </h1>

      <div class="flex flex-wrap">
        <div class="w-1/3 dashboard__card">
          <span>1540</span>
          <div>
            <p>PIPS</p>
          </div>
        </div>
        <div class="w-1/3 dashboard__card">
          <span>15</span>
          <div>
            <p>TP</p>
            <p>Trade</p>
          </div>
        </div>
        <div class="w-1/3 dashboard__card">
          <span>89%</span>
          <div>
            <p>Winning</p>
            <p>Rate</p>
          </div>
        </div>
      </div>
    </div>

    <Table/>
  </div>
</template>

<script>
import Table from "@/components/Table";
export default {
  components: {
    Table
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
