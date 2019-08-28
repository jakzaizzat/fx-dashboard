<template>
  <div class="header">
    <div class="header__title">Overview</div>
    <button class="header__button">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
        <path
          class="heroicon-ui"
          d="M17 11a1 1 0 0 1 0 2h-4v4a1 1 0 0 1-2 0v-4H7a1 1 0 0 1 0-2h4V7a1 1 0 0 1 2 0v4h4z"
        ></path>
      </svg>
      <span class="ml-2">Add New Analysis</span>
    </button>
  </div>
</template>


<style lang="postcss" scoped>
.header {
  @apply p-4 bg-white w-full flex justify-between items-center;
}

.header__title {
  @apply font-medium;
}

.header__button {
  @apply flex items-center bg-green text-white p-2 rounded text-sm shadow;
}

.header__button:hover {
  @apply bg-green-dark;
}

.header__button svg {
  @apply fill-current text-white h-4 w-4;
}
</style>
