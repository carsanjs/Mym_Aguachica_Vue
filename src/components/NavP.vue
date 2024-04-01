<script>


export default{
    name:'NavP',
    data() {
        return {
            
        }
    },
}

</script>
<template>
    <div class="hero-banner">
<section>
<div class="hero-content">
 <h1 class="title comfel comlew">Comparte<em class="emred"> Felicidad</em></h1>
 <h1 class="title comfel comlew">Comparte<em class="emred"> Amor</em></h1>
<a href="#" class="grey__btn primary__btn">Ordena Ahora</a> 
</div>
</section>
<section>
<img src="https://i.ibb.co/0jmb24w/pizza.png" alt="m&m">
</section>
</div>


</template>

<style>
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
}

*,html{
scroll-behavior: smooth;
}

*, *:after, *:before {
--webkit-box-sizing: border-box;
--moz-box-sizing: border-box;
box-sizing: border-box;
}

::-webkit-scrollbar {
height: 12px;
width: 8px;
background: var(--dark);
}
::-webkit-scrollbar-thumb {
background: var(--gray);
--webkit-box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.75);
}
::-webkit-scrollbar-corner {
background: var(--dark);
}
/*HERO BANNER*/
.hero-banner{
width:100%;
display:flex;
align-items:center;
}

.hero-banner section{
width:100%;
height:100vh;
position:relative;
color:var(--white);
}

.hero-banner section:nth-child(1){
background-color:var(--darkgreen);
}

.hero-banner section:nth-child(2){
width:60%;
background-color:var(--darkyellow);
}

.hero-banner .hero-content{
padding:2rem 5rem;
width:100%;
}

.hero-banner .hero-content .title{
font-size:4.5em;
font-weight:200;
}

.hero-banner .hero-content em{
font-weight:600;
}

.hero-banner img{
width:100%;
position:absolute;
left:-30%;
--delay: 0s;
animation: arrows 4s var(--delay) infinite ease-in;
}

.hero-banner .btn1{
display:block;
width:200px;
margin:2vh 0;
}

@media (max-width:1320px){
.hero-banner .hero-content .title{
font-size:3em;
}
}

@media (max-width:820px){
.hero-banner{
display:block;
}
.hero-banner .hero-content{
padding:8rem 1rem;
width:100%;
}
.hero-banner section{
height:50vh;
}
.hero-banner .hero-content .title{
font-size:2em;
}
.hero-banner img{
width:100%;
position:relative;
left:0;
}
.hero-banner section:nth-child(1){
background-image:url("https://i.ibb.co/0jmb24w/pizza.png");
background-size:40% 40%;
background-repeat:no-repeat;
background-position:bottom right;
}
.hero-banner section:nth-child(2){
display:none;
}
}


.primary__btn{
    border-style: none;
    padding: 10px;
    text-decoration: none;
    text-align: center;
    font-family: var(--primary-font);
    font-size: 1.5rem;
    border-radius: 5px;
    cursor: pointer;
}
.hero-content .grey__btn{
    background-color:white!important;
    color: rgb(77 4 4)!important;
    transition: all .6s;
}
.hero-content .grey__btn:hover{
    background-color: rgb(77 4 4 / 65%)!important;
    color: white !important;
}
.emred{
    color: #791316;
}


</style>