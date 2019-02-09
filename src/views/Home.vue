<template>
<div>
  <navbar></navbar>
  <top-header></top-header>
  <div class="container-fluid" style="background-color: rgba(255, 255, 255, 0.65);">
    <como-funziona></como-funziona>
  </div>
</div>
</template>

<script>
import Navbar from '@/components/Navbar'
import TopHeader from '@/components/TopHeader'
import ComoFunziona from '@/components/ComoFunziona'

export default {
  name: 'Home',
  components: { Navbar, TopHeader, ComoFunziona }
}
</script>

<style lang="scss">
</style>
