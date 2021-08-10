<template>
  <h1>STORY ROUTE: {{ this.storySlug }}</h1>
</template>

<script>
export default {
  async asyncData({ params }) {
    const storySlug = params.pathMatch;
    return { storySlug }
  }
}
</script>
