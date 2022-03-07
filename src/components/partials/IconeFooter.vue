<template>
    <li><a href=""></a><i class="fab" :class="ClasseIcone"></i></li>
</template>

<script>
export default {
    name: 'IconeFooter',
    props : {
        'ClasseIcone' : String
    }
}
</script>

<style scoped lang='scss'>
@import 'src/assets/variabili.scss';
li{
        list-style: none;
        display: inline-block;
        margin-left: 65px;
        margin-right: 30px;
        i{
          font-size: 25px;
          color: $colorTitolo;
        }
}
</style>