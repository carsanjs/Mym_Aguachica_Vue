
<script>

export default{
  name:'MenuC',
    data() {
        return {
            title:"Menu M&M",
            searchText:""
        }
    },
}

</script>
<template> 
<div class="divconteform">
  <div class="lefttim"><h1 class="titlemenu">{{ title }}</h1></div>
		<form class="formsearch" v-on:submit.prevent>
			<v-col cols="12" sm="6" md="4">
<v-text-field v-model="searchText" label="" placeholder="Buscar Aqui.." append-icon="search" outlined dense clearable
				></v-text-field>
			</v-col>
		</form>
    </div>
	
<div class="boxes">
<div class="section1">

<div class="section1-card">
<router-link to="/Pizzas">
<div class="sectcont-img"><img src="../../assets/icon/piiza2222.ico" alt="pizzas"></div>
<div class="mnc"><h1 class="ahtime">Pizzas</h1></div></router-link>
</div>
<div class="section1-card">
<router-link to="/Pizzas"><img src="../../assets/icon/rollos.ico" alt="Canelones">
<div class="mnc"><h1 class="ahtime">Canelones</h1></div></router-link>
</div> 
<div class="section1-card">
  <router-link to="/Pizzas"><img src="../../assets/icon/wraps.ico" alt="Wraps">
<div class="mnc"><h1 class="ahtime">Wrasp</h1></div></router-link>
</div>
<div class="section1-card">
  <router-link to="/Pizzas"><img src="../../assets/icon/pastas22.ico" alt="Pastas">
<div class="mnc"><h1 class="ahtime">Pastas</h1></div></router-link>
</div>
<div class="section1-card">
  <router-link to="/Pizzas"><img src="../../assets/icon/ensaladas.ico" alt="Ensaladas">
<div class="mnc"><h1 class="ahtime">Ensaladas</h1></div></router-link>
</div>
<div class="section1-card">
  <router-link to="/Pizzas"><img src="../../assets/icon/hamburguesa.png" alt="Hamburguesas">
<div class="mnc"><h1 class="ahtime">Hamburguesas</h1></div></router-link>
</div>
<div class="section1-card">
  <router-link to="/Pizzas"><img src="../../assets/icon/coctel.ico" alt="Cocteles">
<div class="mnc"><h1 class="ahtime">Cocteles</h1></div></router-link>
</div>
<div class="section1-card">
  <router-link to="/Pizzas"><img src="../../assets/icon/malteadas.ico" alt="Malteadas">
<div class="mnc"><h1 class="ahtime">Malteadas</h1></div></router-link>
</div>
<div class="section1-card">
  <router-link to="/Pizzas">
    <div class="sectcont-img"><img src="../../assets/icon/entradas.ico" alt="Entradas"></div>
<div class="mnc"><h1 class="ahtime">Entradas</h1></div></router-link>
</div>
<div class="section1-card">
  <router-link to="/Pizzas"><img src="../../assets/icon/pollo.ico" alt="Pollos">
<div class="mnc"><h1 class="ahtime">Pollo</h1></div></router-link>
</div>
<div class="section1-card">
<router-link to="/Pizzas"><img src="../../assets/icon/carne.ico" alt="Carnes">
<div class="mnc"><h1 class="ahtime">Carnes</h1></div></router-link>
</div>

</div>
</div> 
</template>

<style scoped>

:root{
scrollbar-color: rgb(210,210,210) rgb(46,54,69) !important;
scrollbar-width: thin !important;
--primary-font: 'Nunito', sans-serif;
--white:#fff;
--black:#000;
--darkgreen:rgb(254 227 172);
--darkyellow:#791316;
--darkred:#9e1414;
--litegreen:#62c08b;
--dark:#242426;
--gray:#5e6f77;
--ligthgray:#f4f4f4;
}

.ahtime{
  color: #282828;
  /* color:rgba(26, 24, 24, 0.836); */
}

.lefttim {
  padding-left: 20px;
}

.mnc{
  margin:1rem;
}

.boxes {
  padding: 0.5rem 0;
  background: #fff;
  box-shadow: 0px 1px 3px 0px rgba(0,0,0,0.25);
  display: grid;
  overflow-x: scroll;
  overflow-y: none;
  justify-items: center;
  border-radius: 5px;
}

/*SECTION1*/
.section1{
  margin: 0.5rem 0;
    padding: 0.5rem 0;
  background-color: #f4f4f4;
  position: relative;  
  display: flex;
  width: 100%;
}

.section1 .section1-card{
background-color:var(--white);
border-radius:10px;
text-align:center;
margin:0.5rem;
width:100%;
box-shadow:0px 4px 8px -4px rgba(1,1,1,0.5);
transition:0.5s;
}

 /* .section1 .section1-card:hover{
box-shadow:0px 1px 2px -1px rgba(1,1,1,0.5);
background-color: #A22020;
}  */

.section1 .section1-card .mnc h1{
font-size:1.3em;
line-height:0;
}

.section1 .section1-card h5{
color:var(--gray);
font-weight:400;
}

/* ************* -----------COMIENZO DE DISEÑOS--RESPONSIVES----*********** */
/* --------------------------------------------------------------------------------- */
@media (max-width:861px){
.section1{
display:block;
width:100%;
top:0;
padding:1rem;
}
.section1 .section1-card{
margin:10px 0;
display:flex;
align-items:center;
}
.section1 .section1-card h5{
display:none;
}
}
/* -------------------------------- */
@media (min-width:430px) and (max-width:860px){
  .boxes {
  width: 100%;
  padding:0px 5px 0px 5px;
  overflow-x: scroll;
  overflow-y: hidden;
}
.section1{
    background-color:#f4f4f4;
    border-radius:10px;
    display: flex;
    align-items: center;
    list-style-type: none;
    margin: 0.5rem 0;
    padding: 0.2rem 0;
}

.section1 .section1-card{
    background-color:var(--white);
    border-radius: 10px;
    padding: 0.5rem 0.5rem;
    text-align: center;
    margin: 0.5rem;
    width: 120px;  
    box-shadow: 0px 4px 8px -4px rgb(1 1 1 / 50%);
    transition: 0.5s;
}
.section1-card a{
  width: 100px;
  display: block;
}

.section1-card a .sectcont-img img {
  width: 100%;
}

.section1 .section1-card .mnc h1{
font-size:1em;
color:red;
line-height:0;
}


}

/* Smartphones (portrait) */
@media only screen and (max-width : 429px) {
  .boxes {
    width: 360px;
  overflow-x: scroll;
  overflow-y: hidden;
  position: fixed;
  top: 0;
  background-color: #fff;
  /* padding: 20px 0;
  /* background: rgb(106, 24, 24); */
  /* box-shadow: 0px 1px 3px 0px rgba(0,0,0,0.25);
  display:flex;
  overflow-x: scroll;
  border-radius: 5px;  */
}

  .section1{
    background: red;
    display: flex;
    align-items: center;
    list-style-type: none;
    margin: 1rem 0;
    padding: 1rem 0;
  /* position: relative;  
  display: flex;
  width: 90%; */
}

}
</style>