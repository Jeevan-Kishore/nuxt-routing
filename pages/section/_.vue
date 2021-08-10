<template>
  <h1>SECTION ROUTE: {{ this.sectionSlug }}</h1>
</template>

<script>
export default {
  async asyncData({ params }) {
    const sectionSlug = params.pathMatch;
    return { sectionSlug }
  }
}
</script>
