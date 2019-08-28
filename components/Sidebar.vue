<template>
  <div class="sidebar">
    <div>
      <div class="sidebar__logo">FinanceLatte</div>
      <div class="sidebar__body">
        <a href="/dashboard" class="sidebar__item">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="icon-dashboard">
            <path
              class="secondary"
              d="M3 11h2a1 1 0 0 1 0 2H3v-2zm3.34-6.07l1.42 1.41a1 1 0 0 1-1.42 1.42L4.93 6.34l1.41-1.41zM13 3v2a1 1 0 0 1-2 0V3h2zm6.07 3.34l-1.41 1.42a1 1 0 1 1-1.42-1.42l1.42-1.41 1.41 1.41zM21 13h-2a1 1 0 0 1 0-2h2v2z"
            ></path>
            <path
              class="primary"
              d="M12 22a10 10 0 1 1 0-20 10 10 0 0 1 0 20zm-6.93-6h13.86a8 8 0 1 0-13.86 0z"
            ></path>
            <path class="secondary" d="M11 14.27V9a1 1 0 0 1 2 0v5.27a2 2 0 1 1-2 0z"></path>
          </svg>
          <span>Dashboard</span>
        </a>
        <a href="/process" class="sidebar__item">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="icon-monitor">
            <path
              class="secondary"
              d="M21 14v5a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-5h3a1 1 0 0 0 .83-.45L10 8.8l5.17 7.75a1 1 0 0 0 1.66 0l1.7-2.55H21z"
            ></path>
            <path
              class="primary"
              d="M21 12h-3a1 1 0 0 0-.83.45L16 14.2l-5.17-7.75a1 1 0 0 0-1.66 0L5.47 12H3V5c0-1.1.9-2 2-2h14a2 2 0 0 1 2 2v7z"
            ></path>
          </svg>
          <span>Process</span>
        </a>
        <a href="/report" class="sidebar__item">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="icon-pie-chart">
            <path
              class="primary"
              d="M14 13h6.78a1 1 0 0 1 .97 1.22A10 10 0 1 1 9.78 2.25a1 1 0 0 1 1.22.97V10a3 3 0 0 0 3 3z"
            ></path>
            <path
              class="secondary"
              d="M20.78 11H14a1 1 0 0 1-1-1V3.22a1 1 0 0 1 1.22-.97c3.74.85 6.68 3.79 7.53 7.53a1 1 0 0 1-.97 1.22z"
            ></path>
          </svg>
          <span>Report</span>
        </a>
      </div>
    </div>
    <div class="sidebar__footer">
      Jakz Aizzat
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        class="icon-cheveron-up"
      >
        <path
          class="secondary"
          fill-rule="evenodd"
          d="M8.7 13.7a1 1 0 1 1-1.4-1.4l4-4a1 1 0 0 1 1.4 0l4 4a1 1 0 0 1-1.4 1.4L12 10.42l-3.3 3.3z"
        ></path>
      </svg>
    </div>
  </div>
</template>

<style lang="postcss" scoped>
.sidebar {
  background-color: #2b323c;
  @apply min-h-screen flex flex-col justify-between;
}

.sidebar__logo {
  background-color: #333c45;

  @apply text-white font-bold text-lg  p-6 tracking-wide;
}

.sidebar__item {
  @apply flex items-center no-underline text-grey-light p-6 py-4;
}

.sidebar__item:hover {
  @apply bg-grey-darkest;
}

.sidebar__item svg {
  @apply h-4 w-4 fill-current text-grey-light;
}
.sidebar__item span {
  @apply pl-3 text-sm;
}

@media (max-width: 768px) {
  .sidebar__item span {
    @apply hidden;
  }
}

.sidebar__footer {
  background-color: #333c45;
  @apply text-white  text-lg  p-6 tracking-wide flex items-center justify-between;
}
.sidebar__footer svg {
  @apply h-6 w-6 fill-current text-grey-light;
}
</style>