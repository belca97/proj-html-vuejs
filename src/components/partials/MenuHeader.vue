<template>

        <li><a href="">{{text}}</a></li>
  
</template>

<script>
export default {
     name: 'MenuHeader',
     props: {
         'text': String,
     }
}
</script>

<style scoped lang='scss'>
@import 'src/assets/variabili.scss';
ul li{
 list-style: none;
 display: inline;
 margin: 0px 20px;
     a{
         text-decoration: none;
         color: $colorMenuHeader;
         padding-bottom: 5px ;
         font-weight: bold;   
         display: inline;      
     }
     
}
 a:hover{
       border-bottom: 2px solid $colorMenuHeader;
 }
</style>