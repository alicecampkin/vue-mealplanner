<template>
  <body>
    <page-header />
    <main class="inner">
      <slot />
    </main>
    <page-footer />
  </body>
</template>

<script>
import PageHeader from "./PageHeader.vue";
import PageFooter from "./PageFooter.vue";

export default {
  components: {
    PageHeader,
    PageFooter,
  },
};
</script>

<style lang="scss" scoped>
body {
  font-family: sans-serif;
  background: #fafafa;
  width: 100vw;
  height: 100vh;
  margin: 0;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

main {
  flex-grow: 1;
  overflow: hidden;
  display: grid;
  grid-template-columns: 300px 1fr 80px;
  column-gap: 1rem;
  padding: 1rem 0;
}
</style>