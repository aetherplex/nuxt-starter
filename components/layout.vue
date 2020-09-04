<template>
  <div class="page-container">
    <div class="content-container">
      <div class="top-content-container">
        <Header />
        <slot name="main"></slot>
      </div>
      <div class="footer-container">
        <Footer />
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./header";
import Footer from "./footer";
export default {
  components: {
    Header,
    Footer
  }
};
</script>

<style lang="scss" scoped>
.page-container {
  width: 100%;
  min-height: 100vh;
}

.content-container {
  width: 90vw;
  max-width: 1200px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
  min-height: 100vh;
}

.top-content-container {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  width: 100%;
  flex-grow: 2;
}

.footer-container {
  flex-grow: 1;
  max-height: 4rem;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
