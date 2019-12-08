<template lang="md">
  <section class="slug">
    <h1 class="slug_title">
      タイトル
    </h1>
    <p class="slug_date">2018/8/2</p>
    <div v-html="$md.render(model)"></div>
  </section>
</template>

<script>
import VueMarkdown from 'vue-markdown'
export default {
  components: {
    VueMarkdown
  },
  data() {
    return {
      model: '- Hello World!'
    }
  }
}
</script>

<style scoped>
.slug {
  max-width: 800px;
  margin: 0 auto;
}
.slug_title {
  font-size: 2.0rem;
  font-weight: bolder;
}
.slug_date {
  font-size: 1.0rem;
  color: rgb(57, 72, 85);
  text-align: right;
}
</style>