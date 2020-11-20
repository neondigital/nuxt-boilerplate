<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">
        {{ this.slug }}
      </h1>
      <div class="links">
        <NuxtLink to="/">Home</NuxtLink>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    async asyncData({ params }) {
      const slug = params.slug // When calling /abc the slug will be "abc"
      return { slug }
    }
  }
</script>