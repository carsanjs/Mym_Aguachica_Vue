<script>
import Cpizza from '../../components/DivMenus/menus/Cpizza.vue';
export default{
    data(){
        name:"pizzas"
        return{

        }
    },
    components:{
        Cpizza
    }
}

</script>

<template>
    <div class="v-spizza">
        <Cpizza/>
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

div.v-spizza{
    display: flex;
    
}


 
/* @media screen and (min-width:268px) and (max-width:429px){
   
}

@media screen and (min-width: 430px) and (max-height:658px){


}

@media screen and  (min-width:412px) and (min-height:914px){
  
}

 @media screen and (min-width: 500px) and (max-height:760px) {
}

@media screen and (min-width:1050px) and (min-height:650px){
}

@media screen and   (min-width:757px) and (min-height: 1500px){
   
} */
</style>