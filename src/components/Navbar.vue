<template>
  <nav class="navbar navbar-light bg-light sticky-top">
    <a class="navbar-brand" href="#">
      <img src="../assets/images/logo.png" height="40" alt="">
    </a>
    <form class="form-inline">
      <button class="btn btn-pide btn-success" type="submit">PIDE AHORA</button>
    </form>
  </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style lang="scss">
.navbar {
  background-color: white !important;
}
.navbar-brand {
  font-weight: bold;
  font-size: 35px;
}
</style>
