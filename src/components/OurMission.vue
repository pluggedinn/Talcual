<template>
<div>
  <div class="container-fluid">
    <div class="row pt-5 pb-5">
      <div class="col-12">
        <h3 class="text-center section-title pb-3">NUESTRA MISSION</h3>
        <p class="text-center">Empezamos buscando a los mejores productores, esos que se dedican a sembrar y cosechar ingredientes sanos, deliciosos y orgánicos, y los encontramos. No sólo los encontramos, nos sentamos a su mesa, viajamos por sus campos y cosechamos de su mano lo mejor de sus tierras. ¿Qué hicimos después? Nos llevamos todo eso a la cocina. ¡A experimentar se ha dicho! Y después de prueba y error (y de comernos todas las pruebas) creamos recetas deliciosas, completas, sanas, de esas que una vez que terminas de comer te sientes feliz y satisfecho. Ahora lo llevamos hasta ti para permitirte ser parte del proceso. Queremos que seas parte de esto, que sepas de dónde viene tu comida, que llegue a ti de la forma más sencilla y que la disfrutes siempre. Eso somos, eso queremos. Tal cual.</p>
      </div>
    </div>
  </div>
  <slick
    ref="mission"
    :options="slickOptionsLg">
    <div class="element" style="background-image: url('../assets/images/mission/s1.jpg');">
      <!-- <img src="../assets/images/mission/s1.jpg"> -->
    </div>
    <div class="element" style="background-image: url('../assets/images/mission/s2.jpg');">
      <!-- <img src="../assets/images/mission/s2.jpg"> -->
    </div>
    <!-- <div class="element">
      <img src="../assets/images/mission/s3.jpg">
    </div>
    <div class="element">
      <img src="../assets/images/mission/s4.jpg">
    </div> -->
  </slick>
</div>
</template>

<script>
import Slick from 'vue-slick'

export default {
  name: 'OurMission',
  components: { Slick },
  data () {
    return {
      slickOptionsLg: {
        infinite: true,
        dots:false, 
        // variableWidth: true,
        centerMode: true, slidesToShow: 1, slidesToScroll: 1, arrows: false
      }
    }
  }
}
</script>

<style lang="scss" scoped>
.slick-slide {
  outline: none;
  width: 300px;
  height: 600px;
}
.element img {
  width: 100%;
  // border: 1px solid black;
  // -webkit-filter: drop-shadow(5px 5px 5px #222);
  // filter: drop-shadow(5px 5px 5px #222);
}
</style>

