<template>
  <main>
    <nuxt-link class="btn block" to="/careers">Careers</nuxt-link>
    <section v-if="posts" class="w-full max-w-5xl mx-auto">
      <h1 class="title">Jobs</h1>
      <posts post-type="jobs" :amount="10" />
    </section>
  </main>
</template>

<script>
export default {
  async asyncData({ $content, error }) {
    let posts
    try {
      posts = await $content('jobs').fetch()
    } catch (e) {
      error({ message: 'Jobs not found' })
    }
    return { posts }
  },
}
</script>
