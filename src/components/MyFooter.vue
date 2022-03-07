<template>

  <footer>
    <div class="container ms_container">
      <div class="ms_left-50">
        <div class="box-logo pb-5">
            <span class="logo">Bakery</span>
            <span class="logo-bottom">AVADA - SHOP</span>
        </div>
        <ul class="pb-5">
          <!-- Menu footer tramite componente esterno -->
          <MenuFooter v-for="(testo, index) in TestiFooter" :key="index"
          :text='testo.text'/>
          <li><a href=""></a><i class="fas fa-shopping-cart"></i><span class="ms_number-footer">0</span></li>
        </ul>
        <p>@ Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved</p>
      </div>
      <div class="ms_right-40 d-flex flex-column align-items-end">
        <p class="pb-5">Subscribe to our Newsletter</p>
        <div class="ms_form w-100">
            <input type="text" placeholder="Enter email adress*">
            <button class="">Subscribe</button>
        </div>
        <div class="icons">
          <ul>
            <!-- Icone footer tramite componente esterno -->
            <IconeFooter v-for="(icona, index) in Icone" :key="index"
            :ClasseIcone="icona.text"/>
          </ul>
        </div>
        <div class="arrow">
            <i class="fas fa-angle-up"></i>       
        </div>
      </div>
        
    </div>

    

  </footer>
</template>

<script>
import MenuFooter from './partials/MenuFooter.vue'
import IconeFooter from './partials/IconeFooter.vue'
export default {
    name: 'MyFooter',
    components:{
      MenuFooter,
      IconeFooter
    },
    data (){
        return{

            //array di oggetti per il menu del footer


            TestiFooter : [
              {
                text : 'Shop'
              },
              {
                text : 'About'
              },
              {
                text : 'Gallery'
              },
              {
                text : 'Locations'
              },
              {
                text : 'Journal'
              },
              {
                text : 'Contact'
              },
              {
                text : 'Orders'
              }
            ],
            Icone : [
              {
                text : 'fa-instagram'
              },
              {
                text : 'fa-twitter'
              },
              {
                text : 'fa-facebook-f'
              },
              {
                text : 'fa-pinterest-p'
              },              
            ]
      }
    }
}
</script>

<style scoped lang='scss'>

  @import '../assets/variabili.scss';




  footer{
    height: 400px;
    /* stilizzazione logo */
    .box-logo{
      height: 150px;
      width: 150px;
      position: relative;
            .logo{
            font-family: 'Lora', serif;
            font-size: 40px;
            font-style: italic;
            color: $colorTitolo;
          }
          .logo-bottom{
            font-size: 10px;
            position: absolute;
            top: 32%;
            left: 21%;
            color: $colorTitolo;
          }
    }
    
  }

  .ms_left-50{
    width: 50%;
    float: left;
    ul{
      padding: 0px 0px;
      li{
      list-style: none;
      display: inline-block;
      color: $colorTitolo;
      padding-right: 15px;
      i{
        margin-right: 10px;
      }
      .ms_number-footer{
        padding: 6px;
        background-color: rgba(161, 159, 159, 0.3);
        border-radius: 30px;
      }
    }
    }
  }
  .ms_right-40{
    float: right;
    width: 40%;
    p{
       color: $colorTitolo;
       font-size: 30px;
    }
    button{
             padding: 3px 15px;
             background-color: $colorTitolo;
             border: 1px solid white;
             border-radius: 8px;
             font-size: 20px;
             color: white;
    }
    input{
      border-radius: 10px;
      padding: 3px 15px;
      width: 73%;
      margin-right: 15px;
    }
    .icons{
      margin-top: 85px;
      ul li{
        list-style: none;
        display: inline-block;
        margin-left: 65px;
        margin-right: 30px;
        i{
          font-size: 25px;
          color: $colorTitolo;
        }
      }
    }
  }
  .arrow{
    background-color: rgb(78, 75, 75);
    color: white;
    height: 50px;
    width: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 10px;
    font-size: 25px;
  }

  .ms_container::after{
    content: '';
    display: table;
    clear: both;
  }

</style>