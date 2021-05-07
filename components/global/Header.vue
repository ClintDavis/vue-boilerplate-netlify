<template>
  <header class="relative flex flex-wrap items-center justify-between px-2 py-3 mb-3">
    <a href="#" class="block">
    <span class="sr-only">BDE Group</span>
      <img class="h-6 md:h-8" src="https://picsum.photos/seed/bde/1200/300" alt="BDE Group" title="BDE Group">
    </a>
    <nav aria-label="Main Menu" class="lg:flex lg:flex-grow items-center">
      <ul class="flex flex-col lg:flex-row list-none ml-auto">
        <li class="nav-item hover:underline">
          <nuxt-link class="btn block" to="/solutions">Solutions</nuxt-link>
        </li>
        <li class="nav-item hover:underline">
          <nuxt-link class="btn block" to="/about">About Us</nuxt-link>
        </li>
        <li class="nav-item hover:underline">
          <nuxt-link class="btn block" to="/news">News</nuxt-link>
        </li>
        <li class="nav-item hover:underline">
          <nuxt-link class="btn block" to="/jobs">Jobs</nuxt-link>
        </li>
        <li class="nav-item hover:underline">
          <nuxt-link class="btn block" to="/contact">Contact</nuxt-link>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style lang="postcss" scoped>
.scrim-bg {
  &::before {
    content: '';
    z-index: -1;
    background-color: var(--bg);
    @apply absolute bottom-0 inset-x-0 h-12 mb-4 transition-colors duration-200 ease-in-out;
  }
  &::after {
    content: '';
    z-index: -1;
    opacity: 1;
    animation: fadeIn1 500ms ease-in-out;
    @apply pointer-events-none absolute bottom-0 inset-x-0 h-16 -mb-12;
    background: linear-gradient(to bottom, #111827, cubic-bezier(0.15, 0, 0.45, 1), transparent);
  }
}
.nuxt-link-exact-active {
  @apply text-gray-200 border-gray-400 bg-gray-800 bg-opacity-25 cursor-default;
}

.light-mode {
  & .scrim-bg {
    &::after {
      animation-name: fadeIn2;
      background: linear-gradient(to bottom, #e5e7eb, cubic-bezier(0.15, 0, 0.45, 1), transparent);
    }
  }
  & .nuxt-link-exact-active {
    @apply text-primary-700 border-gray-600 bg-gray-100;
  }
}

/* Need two because of smoother switching between color modes */
@keyframes fadeIn1 {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes fadeIn2 {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
