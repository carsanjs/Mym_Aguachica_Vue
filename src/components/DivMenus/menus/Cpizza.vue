<script>
export default{
  data(){
    name:"Cpizza"
    return{
            PizzaGrande:[ 
               {
                id:"",
                nombreProducto:"Pizza Hut",
                precio:"21000",
                descuentotext:"Obten Extra 15% Descuento",
                tiempoestimado:"39 mins",
                cantidad:0,
                ingredientes:"Italian, Fast Food, Beverages",
                descuentocount:0,
                puntaje:4.6,
                comprar:"Comprar",
                adiccion:"Adiccionar",
                acarrito:"Agregar",
                domicilios:"DOMICILIOS",
                show:true


               }
          ]
    }
  }
}
</script>

<template>
    <div class = "cards-container">
    <div class = "card" v-for="(next, i) in PizzaGrande" :key="i">
    <div class = "card-media">
        <div class = "discount"><p>{{ next.domicilios }}</p></div>
        <div class = "pro-discount">{{ next.descuentotext }}</div>
        <div class = "delivery-time">{{ next.tiempoestimado }}</div>
        <div class = "bookmark"></div>
      </div>
      <div class = "card-description">
        <div class = "about-place">


          <div class = "place">
          <div class="pl-title"> <p class = "place-name">{{ next.nombreProducto }}</p> </div>
          
            <div class="div-if">
            <div class="das"> <p class = "place-speciality">{{ next.ingredientes }}</p> </div>

            
            <button type="button" v-bind="show">hola</button>
            <span v-if="show = true">primer menu</span>
            <span v-else-if="!show">{{ next.ingredientes }}</span>

            
            </div>


          </div>



          <div class = "place-review">
            <div class="cont-pla-rev">
            <p class = "rating">{{ next.puntaje}} &#x2605; </p></div>
            <div class="cont-pla-rev contdosplarev">
            <p class = "carting"> {{  next.comprar }} &#x24; </p>
            <p class = "acating"> {{ next.acarrito }} &#x271B; </p>
            </div>
            <p class = "per-person"> &#x20b9; 200 per one</p>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<style scoped>
*,
*::after,
*::before{
    padding: 0;
    margin: 0;
    text-decoration: none;
    list-style: none; 
}
.cards-container {
  min-width: 28%;
  max-width: 30%;
  margin: 0 auto;
  padding-top: 10px;
}

.card {
  background-color: #fff;
  box-shadow: 10px 10px 40px 2px rgba(128, 128, 128, 0.4);
  display: inline-block;
  width: 375px;
  border-radius: 10px;
}
.card .card-media {
  background-image: url(https://images.unsplash.com/photo-1615719413546-198b25453f85?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxNDU4OXwwfDF8cmFuZG9tfHx8fHx8fHx8MTYzMDQwMjkwNA&ixlib=rb-1.2.1&q=85);
  background-position: center;
  background-size: cover;
  height: 200px;
  width: 100%;
  object-fit: fit;
  border-radius: 10px 10px 0 0;
  position: relative;
}
.card .card-media .discount {
  background-color: #3582ec;
  position: absolute;
  bottom: 25%;
  padding-left: 4px;
  border-radius: 0 4px 4px 0;
  max-width: 85px;
  left: 0;
}
.card .card-media .discount p {
  font-weight: 400;
  font-size: 13px;
  color: #fff;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
.card .card-media .pro-discount {
font-size: 13px;
background-color: #e83940;
position: absolute;
bottom: 4%;
padding: 3px 4px;
border-radius: 0 4px 4px 0;
max-width: 130px;
left: 0;
color: #fff;
}
.card .card-media .delivery-time {
  position: absolute;
  background-color: #f5f5f5;
  max-width: 60px;
  padding: 3px 6px;
  font-size: 12px;
  right: 3%;
  bottom: 6%;
  border-radius: 4px;
}
.card .card-description {
  padding: 10px;
}
.card .card-description .about-place {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.card .card-description .about-place .place-name {
  font-weight: 600;
  color: rgba(0, 0, 0, 0.87);
}
 .card .card-description .about-place .per-person {
  font-size: 14px;
  text-align: right ;
  padding-right: 5px;
  color: rgba(128, 128, 128, 0.97);
}

.card .card-description .about-place .place .place-speciality{
  padding-right: 3px;
  font-size: 13px;
  color: rgba(128, 128, 128, 0.97);
  text-align: left;
}
.card .card-description .about-place .place-review .rating {
  font-size: 13px;
  border-radius: 4px;
  background-color: #fc5500;
  color: #fff;
  font-weight: 700;
  text-align: center;
  padding: 2px 3px;
  margin-bottom: 6px;
  margin-left: 2px;
  position: relative;
  z-index: 1;
  overflow: hidden;
  display: inline-block;
}
.card .card-description .about-place .place-review .rating:hover {
  transition: all 0.4s ease;
  color:#ffff00;/* color de fuente hover */
}

.card .card-description .about-place .place-review .rating:hover::after {
  transition: all 0.6s ease-out;
  transform: scale(1, 1);
}
.card .card-description .about-place .carting {
font-size: 13px;
border-radius: 4px;
background-color:#009846;
color: #fff;
font-weight: 700;
text-align: center;
padding: 2px 2px;
margin-bottom: 6px;
margin-left: 3px;
position: relative;
  z-index: 1;
  overflow: hidden;
  display: inline-block;
}
.card .card-description .about-place .carting:hover {
  color: #fff; /* color de fuente hover */
}
.card .card-description .about-place .carting::after {
  content: "";
  background: #44be69ea; /* color de fondo hover */
  position: absolute;
  z-index: -1;
  padding: 16px 20px;
  display: block;
  top: 0;
  bottom: 0;
  left: -100%;
  right: 100%;
  -webkit-transition: all 0.35s;
  transition: all 0.35s;
}
.card .card-description .about-place .carting:hover::after {
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  -webkit-transition: all 0.35s;
  transition: all 0.35s;
}

.card .card-description .about-place .acating {
  font-size: 13px;
  border-radius: 4px;
  background-color: #e00000;
  color: #fff;
  font-weight: 700;
  text-align: center;
  padding: 2px 2px;
  margin-bottom: 6px;
  margin-left: 3px;
  position: relative;
  z-index: 1;
  overflow: hidden;
  display: inline-block;
}
.card .card-description .about-place .acating:hover {
  color: #fff; /* color de fuente hover */
}
.card .card-description .about-place .acating::after {
  content: "";
  background:#ff0000; /* color de fondo hover */
  position: absolute;
  z-index: -1;
  padding: 16px 20px;
  display: block;
  top: 0;
  bottom: 0;
  left: 100%;
  right: -100%;
  -webkit-transition: all 0.35s;
  transition: all 0.35s;
}
.card .card-description .about-place .acating:hover::after {
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  -webkit-transition: all 0.35s;
  transition: all 0.35s;
}

.cards-container .card .card-description .about-place .place-review {
  max-width:50%;
}
.cards-container .card .card-description .about-place .place-review .cont-pla-rev {
  max-width: 100%;
  min-width: 50%;
  padding-right: 5px;
  justify-content: right;
  display: flex;
} 


/* ************* -----------COMIENZO DE DISEÑOS--RESPONSIVES----*********** */
/* Smartphones (portrait) */
@media only screen and (max-width : 450px) {
  .cards-container .card {
  min-width: 80%;
  right: 70%;
  position: relative;
  padding-top: 10px;
}

.card {
  background-color: #fff;
  box-shadow: 10px 10px 40px 2px rgba(128, 128, 128, 0.4);
  display: inline-block;
  width: 335px;
  border-radius: 10px;
} 
}
</style>