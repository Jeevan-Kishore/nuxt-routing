<template>
  <h1>STATIC ROUTE: {{ this.staticSlug }}</h1>
</template>

<script>
export default {
  async asyncData({ params }) {
    const staticSlug = params.pathMatch;
    return { staticSlug }
  }
}
</script>
