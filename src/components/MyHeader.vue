<template>
    <header>

        <!-- creazione menu con logo a sinistra e menu a destra -->
        <div class="ms_container">
            <div class="logo-header">
                <img class="h-100 w-100" src="../assets/bakery-logo.jpg" alt="">
                
            </div>
            <div class="menu-header">
                <ul>
                    <!-- creo il menu in alto a destra in maniera dinamica creando un array di oggetti nello script da dove ricavare informazioni di testo -->
                    <li v-for='(testo, index) in TestiHeader' :key="index"><a href="">{{testo.text}}</a></li>
                    <li><a href=""></a></li>
                </ul>
            </div>

        </div>
        <div class="ms-jumbotron">
            <div class="left-jumbotron">
                <p>FRESH E TASTY BAKERY EVERY DAY</p>
                <h1>The Perfect Fresh Bread</h1>
                <p>Cras consequa lectus vestibulum tortor pulivanr, quis euismod nisl varius. Aliquam erat volutpat.
                 Nulllam quis sagittis nibh ac nulla id orci tempor</p>
                <button>Explore our product</button>
            </div>
             <div class="right-jumbotron">

            </div>

        </div>

    </header>
</template>

<script>
export default {
    name:'MyHeader',
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
    background-color: $colorJubmtronHeader;

            .ms_container{
                height: 100px;
                    .logo-header{
                        float: left;
                        width: 15%;
                        height: 100%;
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
                            margin: 0px 20px;
                                a{
                                    text-decoration: none;
                                    color: $colorMenuHeader;
                                    padding-bottom: 5px ;
                                    
                                }
                                
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
                            color: $colorTitolo;
                        }
                        h1{
                            color: $colorTitolo;
                        }
                        p{
                            color : $colorTitolo;
                        }
                }
                .right-jumbotron{
                    width: 77%;
                    float: right;
                    background-image: url('../assets/pexels-maria-orlova-4916562.jpg');
                    background-size: cover;
                    background-position: bottom;
                    height: 100%;
                    border-radius: 10px;
                }
            }
}
.ms-container::after{
    display: table;
    clear: both;
    content: '';
}
  a:hover{
       border-bottom: 2px solid $colorMenuHeader;
 }
 .ms-jumbotron::after{
     display: table;
     content: '';
     clear: both;
 }


</style>