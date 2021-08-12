<template>
  <h1>ISOMORPHIC ROUTE * : {{ this.slug }}</h1>
</template>

<script>
export default {
  async asyncData({ params }) {
    const slug = params.pathMatch;
    /* TODO: Make calls sequentially to API and return when it's not a 404 / 500, render related template */
    return { slug }
  }
}
</script>
