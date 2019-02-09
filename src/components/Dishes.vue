<template>
<div>
  <div class="container-fluid">
      <div class="row align-items-center p-5">
        <div class="col-12">
          <h3 class="section-title">MENU DE LA SEMANA</h3>
        </div>
      <div class="col-12">
      </div>
    </div>
  </div>
  <slick
    ref="slick"
    :options="slickOptionsLg">
    <div class="element text-center">
      <img src="../assets/images/p1.png">
      <div class="content">
        <h5>Del Mar</h5>
        <p>Jurel en salsa de soya, col de bruselas, frijoles blancos con apio, ensalada de espinacas y betabel, salsa zanahoria jengibre</p>
        <p>$ 180</p>
        <button class="btn btn-pide btn-success" type="submit">PIDE AHORA</button>
      </div>
    </div>
    <div class="element text-center">
      <img src="../assets/images/p2.png">
      <div class="content">
        <h5>De la Tierra</h5>
        <p>Lentejas con comino, ensalada de col verde con espinajas , con camote horneado y salsa de aguacate</p>
        <p>$ 150</p>
        <button class="btn btn-pide btn-success" type="submit">PIDE AHORA</button>
      </div>
    </div>
    <div class="element text-center">
      <img src="../assets/images/p3.png">
      <div class="content">
        <h5>Del campo</h5>
        <p>Rollos de col con requeson, Ensalada de Brocolini, calabasa horneada, base de frijoles, salsa mayonesa de la casa</p>
        <p>$ 180</p>
        <button class="btn btn-pide btn-success" type="submit">PIDE AHORA</button>
      </div>
    </div>
    <div class="element text-center">
      <img src="../assets/images/p4.png">
      <div class="content">
        <h5>Del Santo</h5>
        <p>Lentejas con requeson, verde con espinajas, salsa zanahoria jengibre</p>
        <p>$ 160</p>
        <button class="btn btn-pide btn-success" type="submit">PIDE AHORA</button>
      </div>
    </div>
  </slick>
</div>
</template>

<script>
import Slick from 'vue-slick'

export default {
  name: 'Dishes',
  components: { Slick },
  data () {
    return {
      slickOptionsLg: {
        infinite: false,
        dots:true, 
        centerMode: true, slidesToShow: 3, slidesToScroll: 1, arrows: false
      },
      slickOptionsSm: {
        infinite: false,
        dots:true,
        centerMode: true, slidesToShow: 1, slidesToScroll: 1, arrows: false
      },
      currentOptions: null
    }
  },
  mounted: function () {
    this.currentOptions = this.slickOptionsLg
  }
}
</script>

<style lang="scss">
.content h5 {
  font-weight: bold;
}
.element img {
  margin: 0 auto;
  margin-bottom: 60px;
  width: 90%;
  border: 1px solid black;
  -webkit-filter: drop-shadow(5px 5px 5px #222);
  filter: drop-shadow(5px 5px 5px #222);
}
.slick-center img{
  transition: all 150ms;
  transform: scale(1.1);
}
.slick-slide {
  outline: none;
}
.slick-slide > div {
  visibility: hidden;
  opacity: 0;
}
.slick-center > div {
  transition: opacity 1s ease-out;
  opacity: 1;
  visibility: visible;
}

/* Slick DOTS */
.slick-dots {
  position: absolute;
  top: -30px;
  display: block;
  width: 100%;
  padding: 0;
  margin: 0;
  list-style: none;
  text-align: center;
}
.slick-dots li {
  position: relative;
  display: inline-block;
  width: 20px;
  height: 20px;
  margin: 0 10px;
  padding: 0;
  cursor: pointer;
}
.slick-dots li button {
  outline: none;
  background-color: lightgray;
  color: black;
  width: 25px; height: 25px;  
  border-radius: 50%;
  border: 0;
  cursor: pointer;
}
.slick-dots li.slick-active button {
  background-color: black;
  opacity: 0.7;
  color: white;
}
</style>
