<template>
  <h1>ISOMORPHIC ROUTE * : {{ this.slug }}</h1>
</template>

<script>
export default {
  async asyncData({ params }) {
    const slug = params.pathMatch;
    return { slug }
  }
}
</script>
