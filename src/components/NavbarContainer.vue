<template>
  <div class="navbar">
    <picture>
      <source
        srcset="~@/assets/logo-dark-mode.svg"
        media="(prefers-color-scheme: dark)"
      />
      <source
        srcset="~@/assets/logo-white-mode.svg"
        media="(prefers-color-scheme: light), (prefers-color-scheme: no-preference)"
      />
      <img
        src="~@/assets/logo-dark-mode.svg"
        loading="lazy"
        alt="Tribecamp Logo"
        class="logo"
      />
    </picture>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.navbar {
  padding: 25px;

  .logo {
    width: 130px;
  }
}
</style>
