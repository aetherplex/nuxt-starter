<template>
  <nav class="nav">
    <NuxtLink to="/">
      <h1>Starter</h1>
    </NuxtLink>
    <ul class="routes">
      <NuxtLink to="/about">About</NuxtLink>
      <NuxtLink to="/contact">Contact</NuxtLink>
    </ul>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.nav {
  width: 100%;
  height: 6rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid #ccc;
  margin-bottom: 2rem;
}

.routes {
  & > *:not(:first-child) {
    margin-left: 2rem;
  }
}
</style>
