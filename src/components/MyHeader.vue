<template>
    <header>

        <!-- creazione menu con logo a sinistra e menu a destra -->
        <div class="ms_container">
            <div class="logo-header">
                <div class="box-logo">
                    <span class="logo">Bakery</span>
                    <span class="logo-bottom">AVADA - SHOP</span>
                </div>                
            </div>
            <div class="menu-header px-4">
                <ul>
                    <!-- creo il menu in alto a destra in maniera dinamica creando un array di oggetti nello script da dove ricavare informazioni di testo -->
                    <MenuHeader v-for='(testo, index) in TestiHeader' :key="index"
                    :text="testo.text"/>
                    <li><i class="fas fa-shopping-cart"></i></li>
                </ul>

            </div>

        </div>
        <div class="ms-jumbotron">
            <div class="left-jumbotron">
                <p class="first-p">FRESH E TASTY BAKERY EVERY DAY</p>
                <h1>The Perfect Fresh Bread</h1>
                <p>Cras consequa lectus vestibulum tortor pulivanr, quis euismod nisl varius. Aliquam erat volutpat.
                 Nulllam quis sagittis nibh ac nulla id orci tempor</p>
                <button>Explore our product</button>
            </div>
             <div class="right-jumbotron">
                 <div class="ms_demos">
                     <i class="fab fa-apple"></i>                    
                     <span>Demos</span>
                 </div>
                 <div class="ms_sale">
                     <div class="ms_dollar">$</div>
                     <div class="ms_price">39</div>
                     <span>On Sale</span>
                 </div>
            </div>

        </div>

    </header>
</template>

<script>
import MenuHeader from './partials/MenuHeader.vue'
export default {
    name:'MyHeader',
    components: {
        MenuHeader
    },
    data (){
        return{

            //array di oggetti per il menu dell'header


              TestiHeader : [
              {
                text : 'HOME'
              },
              {
                text : 'SHOP'
              },
              {
                text : 'ABOUT'
              },
              {
                text : 'GALLERY'
              },
              {
                text : 'LOCATIONS'
              },
              {
                text : 'JOURNAL'
              },
              {
                text : 'CONTACT'
              },
              {
                text : 'MY ACCOUNT'
              }
            ],
      }
    }
}
</script>

<style scoped lang='scss'>

@import '../assets/variabili.scss';

header{
    height: 700px;
    background-color: $colorJumbotronHeader;

            .ms_container{
                height: 100px;
                    .logo-header{
                        float: left;
                        width: 15%;
                        height: 100%;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                    }
                    .menu-header{
                        float: right;
                        width: 60%;
                        height: 100%;
                        display: flex;
                        align-items: center;
                        justify-content: flex-end;
                        ul li{
                            list-style: none;
                            display: inline;
                        }
                    }
            }

            .ms-jumbotron{
                height: 600px;
                padding-left: 60px;
                .left-jumbotron{
                    width: 23%;
                    float: left;
                    padding-top: 90px;

                        button{
                            padding: 10px 32px;
                            background-color: white;
                            border: 1px solid white;
                            border-radius: 8px;
                            font-size: 20px;
                            font-weight: bold 700;
                            color: $colorTitolo;
                        }
                        h1{
                            color: $colorTitolo;
                            font-weight: bold;
                        }
                        p{
                            color : $colorParagrafi;
                        }
                        .first-p{
                            font-size: 13px;
                            font-weight: bold 700;
                        }
                }
                .right-jumbotron{
                    width: 74%;
                    float: right;
                    background-image: url('../assets/pexels-maria-orlova-4916562.jpg');
                    background-size: cover;
                    background-position: bottom;
                    height: 100%;
                    border-radius: 10px;
                    position: relative;                    
                    .ms_demos{
                        position: absolute;
                        background-color: white;
                        width: 70px;
                        height: 70px;
                        top: 5%;
                        right: 1%;
                        border-radius: 10px;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        flex-direction: column;
                        font-size: 13px;
                        i{
                            font-size: 30px;
                        }
                    }
                    .ms_sale{
                        position: absolute;
                        background-color: white;
                        width: 70px;
                        height: 70px;
                        top: 18%;
                        right: 1%;
                        border-radius: 10px;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        flex-direction: column;
                        font-size: 13px;
                        .ms_dollar{
                            position: absolute;
                            left: 20%;
                            top: 10%;
                            font-size: 20px;
                            color: rgb(82, 209, 124);
                            font-weight: bold;
                        }
                        .ms_price{
                            font-size: 20px;
                            color: rgb(82, 209, 124);
                            font-weight: bold;    
                            padding-left: 10px;                        
                        }
                    }
                }
            }
}
.ms-container::after{
    display: table;
    clear: both;
    content: '';
}
 .ms-jumbotron::after{
     display: table;
     content: '';
     clear: both;
 }

 .box-logo{
      position: relative;
      height: 90%;
            .logo{
            font-family: 'Lora', serif;
            font-size: 40px;
            font-style: italic;
            color: $colorTitolo;
          }
          .logo-bottom{
            font-size: 10px;
            position: absolute;
            top: 52%;
            left: 21%;
            color: $colorTitolo;
          }
    }

</style>