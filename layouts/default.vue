<template>
  <div class="root">
    <div class="w-1/5">
      <Sidebar/>
    </div>
    <div class="w-4/5">
      <Header/>
      <nuxt/>
    </div>
  </div>
</template>

<script>
import Sidebar from "@/components/Sidebar";
import Header from "@/components/Header";
export default {
  components: {
    Header,
    Sidebar
  }
};
</script>


<style lang="postcss" scoped>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.root {
  background-color: #f1f2f6;
  @apply bg-grey-light min-h-screen flex flex-wrap;
}
</style>
