<template>
<div>
  <navbar></navbar>
  <top-header></top-header>
  <como-funziona></como-funziona>
  <dishes></dishes>
</div>
</template>

<script>
import Navbar from '@/components/Navbar'
import TopHeader from '@/components/TopHeader'
import ComoFunziona from '@/components/ComoFunziona'
import Dishes from '@/components/Dishes'

export default {
  name: 'Home',
  components: { Navbar, TopHeader, ComoFunziona, Dishes }
}
</script>

<style lang="scss">
</style>
