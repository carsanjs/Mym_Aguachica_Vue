
<script>
export default{
    name:'FooterT',
    data() {
        return {
            
        }
    },
}

</script>

<template> 
  
<footer class="footer">
            <div class="all__lists">
                <ul class="list">
                    <div> <h1> Ordenar Ahora</h1></div>
                    <li class="item">
                        <a href="#" class="link">Entradas</a>
                    </li>
                    <li class="item">
                        <a href="#" class="link">Pizzas</a>
                    </li>
                    <li class="item">
                        <a href="#" class="link">Hamburguesas</a>
                    </li>
                    <li class="item">
                        <a href="#" class="link">Platos Fuertes</a>
                    </li>
                    <li class="item">
                        <a href="#" class="link">Pastas</a>
                    </li>
                    <li class="item">
                        <a href="#" class="link">Lasañas</a>
                    </li>
                    <li class="item">
                        <a href="#" class="link">Ensaladas</a>
                    </li>
             
                </ul>
                <ul class="list">
                    <div> <h1> Sobre Nosotros</h1></div>
                    <li class="item">
                        <a href="#" class="link">Acerca de nosotros</a>
                    </li>
                    <li class="item">
                        <a href="#" class="link">Nutricion</a>
                    </li>
                </ul>
                <ul class="list">
                    <div> <h1> Politicas</h1></div>   
                    <li class="item">
                        <a href="#" class="link">Terminos & Condiciones</a>
                    </li>
                </ul>

                <ul class="list">
                    <div> <h1>Visita MyM P´B</h1></div>                   
                    <li class="item">
                        <a href="#" class="link">Localizador Tiendas</a>
                    </li>
                    <li class="item">
                        <a href="#" class="link">Global Blog</a>
                    </li>
                </ul>
            </div>

            <div class="all__lists--2">
                <ul class="list">
                        <li class="item">
                            <a href="#" class="link">Visitanos</a>
                        </li>
                        <li class="item">
                            <a href="#" class="link">Pide ahora</a>
                        </li>
                        <li class="item">
                            <a href="#" class="link">Siguenos</a>
                        </li>
                        <li class="item">
                            <a href="#" class="link">Acerca Nosotros</a>
                        </li>
                </ul>
                <ul class="list">
                        <li class="item">
                            <a href="#" class="link">Registrate</a>
                        </li>
                        <li class="item">
                            <a href="#" class="link">Global Blog</a>
                        </li>
                </ul>
                <ul class="list">
                        <li class="item">
                            <a href="#" class="link">Terminos & Condiciones</a>
                        </li>
                        <li class="item">
                            <a href="#" class="link">Nutricion</a>
                        </li>
                </ul>
            </div>

            <div class="footer__center">
                <div class="feedback">
                    <h2>Ayúdanos a servirte mejor</h2>
                    <button class="grey__btn primary__btn">Comentar</button>
                </div>
                <div class="social">
                    <h2>Síguenos</h2>
                    <ul class="social__icon">
                        <li class="social__icon--item fbk">
                            <a href="#" class="social__icon--link">
                                <i class="fab fa-facebook-f"></i>
                            </a>
                        </li>
                        <li class="social__icon--item twr">
                            <a href="#" class="social__icon--link">
                                <i class="fab fa-twitter"></i>
                            </a>
                        </li>
                        <li class="social__icon--item itgm">
                            <a href="https://www.instagram.com/mymrestaurantes/" class="social__icon--link">
                                <i class="fab fa-instagram"></i>
                            </a>
                        </li>
                        <li class="social__icon--item ytb">
                            <a href="#" class="social__icon--link">
                                <i class="fab fa-youtube"></i>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>     
<section>
 <div class="section5">
 <div class="download">
 <h2 class="h2Dap">Descarga App</h2>
 <span class="mobile">
 <img src="https://www.freepngimg.com/thumb/android/58666-play-google-button-now-app-store.png" alt="ios" srcset="" width="200px">
 <img src="https://www.freepngimg.com/thumb/android/67006-app-play-google-android-store-free-clipart-hd.png" alt="android" srcset="" width="200px">
 </span>
</div>
 <div class="copyright rigthpyco">
  <p class="mefop">© 2022,Restaurante Bar MyM<small>,</small>Todos los derechos reservados</p>
  <p>Pida una deliciosa pizza sobre la marcha, en cualquier lugar y en cualquier momento. Restaurante Bar MyM  es feliz para ayudarle con su entrega a domicilio. Cada vez que ordenas, obtienes un y pizza fresca entregada en su puerta en menos de treinta minutos. Aceptamos Tarjetas Credito u Debito</p>
   <p>¡Date prisa y haz tu pedido ahora!</p>
</div> 
</div>
           
</section>      
</footer>
</template>

<style >

:root{
    --primary-txt-color: white;
    --primary-bg-color: rgb(67, 158, 6);
    --primary-grey-light: silver;
    --primary-grey-dark: grey;
    --primary-font: 'Nunito', sans-serif;
    --hr-font: 'Anton', sans-serif;
}

*,
*::after,
*::before{
    padding: 0;
    margin: 0;
    text-decoration: none;
    list-style: none; 
}

html{
    box-sizing: inherit;
    font-size: 62.5%;
    font-family: var(--primary-font);
}

body{
    box-sizing: border-box;
    overflow-x: hidden;
}

img{
    object-fit: cover;
}

.primary__btn{
    border-style: none;
    padding: 10px;
    text-decoration: none;
    background-color: var(--primary-bg-color);
    text-align: center;
    font-family: var(--primary-font);
    font-size: 1.5rem;
    border-radius: 5px;
    cursor: pointer;
}

/* -------------------------------------------------------------FOOTER SECTION STARTS HERE------------------------------------------------------ */

.footer{
    margin-top: 0.5rem;
    border-radius: 5px;
    border: none;
    color:#791316;
    background-color:#fee3ac;
}

@media only screen and (max-width:990px){
    .footer{
        position: relative;
    }
}

.all__lists{
    padding-top: 3rem;
    width:70%;
    margin: 2rem auto;
    display: flex;
    flex-wrap: wrap;
}

.all__lists > ul{
    margin: 0 auto;
    font-size: 1rem;
}

.all__lists > ul li a{
    font-size: 1.2rem;
    color:#791316;
}

.footer__center{
    display: flex;
    width: 70%;
    margin: 0 auto 2rem auto;
    justify-content: space-between;
}

.feedback{
    display: flex;
    align-items: center;
}

.feedback h2{
    margin: 10px;
}

.feedback .grey__btn{
    background-color:white!important;
    color: rgb(77 4 4)!important;
    transition: all .6s;
}

.feedback .grey__btn:hover{
    background-color: rgb(77 4 4 / 65%)!important;
    color: white !important;
}

.social{
    display: flex;
    flex-direction: column;
    width: 20%;
    text-align: center;
}

.social__icon{
    display: flex;
    margin-top: 1rem;
}

.social__icon .social__icon--item{
    margin: 0 10px;
    width: 20%;
}

    .social__icon .social__icon--item .social__icon--link i{
        font-size: 3rem;
        color: var(--primary-txt-color);
        transition: all .5s;
        border-radius: 10px;
    }


    .social__icon .social__icon--item.fbk:hover i{
        color:#0a81ed!important;
    }
    .social__icon .social__icon--item.twr:hover i{
        color:#0095f6!important;
    }
    .social__icon .social__icon--item.itgm:hover i{
        border-radius: 10px;
        color: -webkit-radial-gradient(32% 106%, circle cover, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), -webkit-linear-gradient(-45deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%);
    background: -moz-radial-gradient(32% 106%, circle cover, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), -moz-linear-gradient(-45deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%);
    background: -ms-radial-gradient(32% 106%, circle cover, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), -ms-linear-gradient(-45deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%);
    background: -o-radial-gradient(32% 106%, circle cover, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), -o-linear-gradient(-45deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%);
    background: radial-gradient(circle farthest-corner at 32% 106%, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), linear-gradient(135deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%)!important;
    }
    .social__icon .social__icon--item.ytb:hover i{
        color: red!important;
    }
@media only screen and (max-width:990px){
    .footer__center{
        display: flex;
        flex-direction: column;
        margin: 0 auto;
        padding-bottom: 1rem;
    }

    .feedback{
        order: 2;
        display: flex;
        flex-direction: column;
    }

    .social{
        width: 100%;
        text-align: center;
        order: 1;
        display: flex;
        flex-direction: column;
    }
}

.download{
    display: none;
}

.copyright{
    border:none;
    position: relative;
    top: 46%;
    margin: 0 auto;
    border-radius: 10px;
    background: rgb(77 4 4 / 65%);
    margin: 0 auto;
    width: 70%;
    font-size: 1.0rem;
    text-justify: auto;
    text-align: center;
}
.h2Dap{
    color: white;
    padding: 0 2rem;
    margin-bottom: 1rem;
    font-family: 'Chivo Mono', monospace;
}

.copyright p{
    color: white;
    padding: 0 2rem;
    margin-bottom: 1rem;
    font-family: 'Chivo Mono', monospace;
}

@media only screen and (max-width:990px){
    .copyright p:not(:first-child){
        display: none;
    }
}

.all__lists--2{
    width: 100%;
    display: none;
}

.all__lists--2 ul{
    margin: 1rem;
    width: inherit;
}

.all__lists--2 ul:first-child{
   border-right: 1px solid var(--primary-txt-color);
   font-weight: bold;
}

.all__lists--2 ul li a{
color:#791316;
    font-size: 1.5rem;
}

@media only screen and (max-width:990px){
    .all__lists{
        display: none;
    }

    .all__lists--2{
        display: flex;
    }

    .download{
        display: flex;
        flex-direction: column;
        text-align: center;
    }

    .download *{
        margin: 0 auto;
    }

    .download h2{
        width: 100%;
        margin-bottom: 1rem;
    }

    .download .mobile{
        width: 100%;
        margin-bottom: 1rem;
    }

    .copyright{
    border:none;
    position: relative;
    top: 46%;
    margin: 0 auto;
    border-radius: 10px;
    background: rgb(77 4 4 / 65%);
    margin: 0 auto;
    width: 70%;
    font-size: 1.0rem;
    text-justify: auto;
    text-align: center;
}
.h2Dap{
    color: white;
    padding: 0 2rem;
    margin-bottom: 1rem;
    font-family: 'Chivo Mono', monospace;
}

.copyright p{
    color: white;
    padding: 0 2rem;
    margin-bottom: 1rem;
    font-family: 'Chivo Mono', monospace;
}
section .section5 .mefop{
    position: absolute;
    background: rgb(77 4 4 / 65%);
    bottom:30px;
}
.rigthpyco .mefop{
    font-size: 15px;
}
}


.fa-twitter:before {
    content: "\f099";
}
.fa-instagram:before {
    content: "\f16d";
}
.fa-youtube:before {
    content: "\f167";
}
/* -------------------------------------------------------------FOOTER SECTION ENDS HERE------------------------------------------------------ */

/*SECTION5*/
.section5{
width:100%;
background-position-y: center;
background-image:url("../assets/img/myg.png");
background-size:cover;
aspect-ratio:  500/ 250;

}

.section5 section{
width:70%;
padding:3rem;
text-align:center;
color:var(--white);
margin:auto;
}

.section5 section h1{ 
font-size:2em;
}

.section5 section h3{ 
font-size:1.6em;
color:var(--white);
font-weight:200;
}

.flex {
display: flex;
align-items: center;
justify-content: center;
}

.app-btn {
white-space:nowrap;
color:#791316;
margin: 20px 10px;
padding:0 0.5rem;
text-align: left;
border-radius: 5px;
text-decoration: none;
font-family: "Lucida Grande", sans-serif;
font-size: 10px;
text-transform: uppercase;
}
.app-btn.blu {
background-color: #101010;
transition: background-color 0.25s linear;
}
.app-btn.blu:hover {
background-color: #454545;
}
.app-btn i {
width: 20%;
text-align: center;
font-size: 28px;
margin-right: 7px;
}
.app-btn .big-txt {
font-size: 17px;
text-transform: capitalize;
}

@media (max-width:920px){
.section5 section{
width:100%;
padding:1rem;
}
.social__icon .social__icon--item .social__icon--link i{
        font-size: 3rem;
        color: var(--primary-txt-color);
        transition: all .5s;
        border-radius: 10px;
    }


    .social__icon .social__icon--item.fbk:hover i{
        color:#0a81ed!important;
    }
    .social__icon .social__icon--item.twr:hover i{
        color:#0095f6!important;
    }
    .social__icon .social__icon--item.itgm:hover i{
        border-radius: 10px;
        color: -webkit-radial-gradient(32% 106%, circle cover, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), -webkit-linear-gradient(-45deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%);
    background: -moz-radial-gradient(32% 106%, circle cover, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), -moz-linear-gradient(-45deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%);
    background: -ms-radial-gradient(32% 106%, circle cover, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), -ms-linear-gradient(-45deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%);
    background: -o-radial-gradient(32% 106%, circle cover, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), -o-linear-gradient(-45deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%);
    background: radial-gradient(circle farthest-corner at 32% 106%, rgb(255, 225, 125) 0%, rgb(255, 205, 105) 10%, rgb(250, 145, 55) 28%, rgb(235, 65, 65) 42%, transparent 82%), linear-gradient(135deg, rgb(35, 75, 215) 12%, rgb(195, 60, 190) 58%)!important;
    }
    .social__icon .social__icon--item.ytb:hover i{
        color: red!important;
    }
}


</style>