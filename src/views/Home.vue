<template>
<div>
  <navbar></navbar>
  <top-header></top-header>
  <our-mission></our-mission>
  <filosofia></filosofia>
  <!-- <como-funziona></como-funziona> -->
  <!-- <dishes></dishes> -->
  <Footer></Footer>
</div>
</template>

<script>
import Navbar from '@/components/Navbar'
import TopHeader from '@/components/TopHeader'
import OurMission from '@/components/OurMission'
import Filosofia from '@/components/Filosofia'
import ComoFunziona from '@/components/ComoFunziona'
import Dishes from '@/components/Dishes'
import Footer from '@/components/Footer'

export default {
  name: 'Home',
  components: { Navbar, TopHeader, OurMission, Filosofia, ComoFunziona, Dishes, Footer }
}
</script>

<style lang="scss">
</style>
