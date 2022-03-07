<template>
  <li><a href="">{{text}}</a></li>
</template>

<script>
export default {
    name:'MenuFooter',
    props : {
        'text' : String
    }
}
</script>

<style scoped lang='scss'>
@import 'src/assets/variabili.scss';
ul{
      padding: 0px 0px;
      li{
      list-style: none;
      display: inline-block;
      color: $colorTitolo;
      padding-right: 15px;
      a{
         text-decoration: none;
         color: $colorParagrafi;
         padding-bottom: 5px ;  
         display: inline;      
     }
 }
}
</style>