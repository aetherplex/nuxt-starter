<template>
  <Layout>
    <template v-slot:main class="container">
      <main>
        <h1>Contact</h1>
      </main>
    </template>
  </Layout>
</template>

<script>
import Layout from "~/components/layout";
export default {
  components: {
    Layout
  }
};
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 100%;
  height: 100%;
}
</style>
