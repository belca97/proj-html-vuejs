<template>
  <main>
    <ComponentMainFirst></ComponentMainFirst>
      <!-- inizio seconda parte main in maniera statica -->
  <div class="container ms_container mt-5">
        <div class="text-center text-second-part">
            <span>CORPORATE E WEDDINGS</span>
            <p>Baking Special Moments</p>
        </div>
        <img class="w-100" src="../assets/hover-img1.png" alt="">
  </div>
       <!-- fine seconda parte main statico -->
       <!-- inizio terza parte main statico -->
       <ComponentMainThird/> 
      <!-- fine terza parte main statico -->
      <!-- inizio quarta parte main statico -->
      <ComponentMainFourth/>
        <!-- fine quarta parte main statico -->
            <!-- inizio quinta parte main statico -->
      <ComponentMainFifth/>
              <!--fine quinta parte main statico -->
              <!-- inizio sesta parte main statico -->
          <div class="ms_container-80 background-img-bread-2 p-5 text-white">
               <div class="top-text-01">
                  <div class="text-left">
                    <p>Delivered To Your Home</p>
                  </div>
                  <div class="text-right">
                    <span>03</span>
                  </div>
               </div>
                <div class="text-bottom-left h-75 w-50">
                  <span class="pb-3">BAKED TO ORDER & GIFT WRAPPED</span>
                  <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Qui dolorem nam quas autem nesciunt molestias cumque itaque illum corrupti odio aliquid quam atque, unde veritatis laborum dolore suscipit recusandae porro?</p>
                </div>
          </div>
          <!-- fine sesta parte main statico -->
          <!-- inizio settima parte main statico -->
          <div class="ms_container-80-2 text-center mt-5 py-5">
            <span>LOCATIONS</span>
            <h3 class="pt-5 ms_style-h">Visit our Bakeries</h3>
            <div class="ms_container">
              <div class="img-left">
                <img class="w-100" src="../assets/pexels-daria-shevtsova-1070946.jpg" alt="">
                <div class="ms_background-grey">
                  <h3 class="py-4 ms_style-h">New York</h3>
                    <div class="px-5 w-100 d-flex align-items-center justify-content-between" >
                      <div>
                        <span>CALL US</span>
                        <p>1.800.458.556</p>
                      </div>
                      <div>
                        <span>OPEN ALL WEEK</span>
                        <p>9.00 AM - 6:00 pm</p>
                      </div>
                      <div>
                        <button>View Map</button>
                      </div>
                </div>
                </div>

                </div>
                <div class="img-right">
                      <img class="w-100" src="../assets/pexels-annam-w-1047458.jpg" alt="">
                      <div class="ms_background-yellow">
                              <h3 class="py-4 ms_style-h">London</h3>
                          <div class="px-5 w-100 d-flex align-items-center justify-content-between" >
                              <div>
                                <span>CALL US</span>
                                <p>1.800.458.556</p>
                              </div>
                              <div>
                                <span>OPEN ALL WEEK</span>
                                <p>9.00 AM - 6:00 pm</p>
                              </div>
                              <div>
                                <button>View Map</button>
                              </div>
                          </div>
                      </div>
                </div>
            </div>

          </div>
          <!-- fine settima parte main statico -->
          <!-- inizio ottava parte main statico -->
           <div class="ms_container-80 ms-container mt-5">
            <div class="img-top-part">
              <div class="ms_float-23">
                <img class="w-100" src="../assets/img-ottava-parte/pexels-anna-shvets-5964505.jpg" alt="">

              </div>
              <div class="ms_float-46 d-flex flex-column justify-content-center align-items-center">
                <span class="pb-3">MADE FOR SHARING</span>
                <h3 class="ms_style-h pb-3">Let's stay in touch</h3>
                <button><i class="fab fa-instagram"></i> Follow us</button>

              </div>
              <div class="ms_float-23">
                <img class="w-100" src="../assets/img-ottava-parte/pexels-katerina-holmes-5910791.jpg" alt="">
              </div>
            </div>
            <div class="img-bottom-part">
              <div class="ms_float-23">
                <img class="w-100" src="../assets/img-ottava-parte/pexels-meruyert-gonullu-6152263.jpg" alt="">
              </div>
             <div class="ms_float-23">
               <img class="w-100" src="../assets/img-ottava-parte/pexels-elle-hughes-5764066.jpg" alt="">
              </div>
              <div class="ms_float-23">
                <img class="w-100" src="../assets/img-ottava-parte/pexels-gustavo-fring-7447284.jpg" alt="">
              </div>
              <div class="ms_float-23">
                <img class="w-100" src="../assets/img-ottava-parte/pexels-tara-winstead-6479556.jpg" alt="">
              </div>
            </div>

          </div>
          <!-- fine ottava parte main statico -->
          <!-- inizio nona parte main statico -->
          <div class="background-img-bread-3 mt-5 mb-5">
            <div class="container h-100">
                  <div class="w-50 h-100 d-flex flex-column justify-content-center align-items-start">
                      <span class="pb-3">TRY OUR SEASONAL PRODUCTS</span>
                      <p class="ms_style-h text-white pb-3">Order for pick-up or delivery to <br> your home</p>
                      <button class="ms_button-white">Shop Now</button>
                </div>
            </div>
          </div>
          <!-- fine nona parte main statico -->

  </main>
</template>

<script>
import ComponentMainFirst from './partials/ComponentMainFirst.vue'
import ComponentMainThird from './partials/ComponentMainThird.vue'
import ComponentMainFourth from './partials/ComponentMainFourth.vue'
import ComponentMainFifth from './partials/ComponentMainFifth.vue'
export default {
    name:'MyMain',
    components : {
      ComponentMainFirst,
      ComponentMainThird,
      ComponentMainFourth,
      ComponentMainFifth,
  }
}


</script>

<style scoped lang='scss'>

  @import '../assets/variabili.scss';
  main{
    margin-top: 100px;
    }
    /*inizio seconda parte del main in maniera statica */

  .text-second-part{
    height: 100px;
    span{
       color: $colorTitolo;
       font-size: 10px;
    }
    p{
       color: $colorTitolo;
       font-size: 30px;
       margin: 20px 0px;
    }
  }

   /*fine seconda parte del main in maniera statica */

   /* inizio sesta parte del main */
   

  .top-text-01::after{
      clear: both;
      content: '';
      display: table;
    }
    .top-text-01{
      height: 100px;
        .text-left{
          float: left;
          width: 50%;
          text-align: left;
          padding-left: 10px;
          p{
            color: white;
            font-size: 30px;
            font-weight: bold;
          }
        }
        .text-right{
          float: right;
          width: 10%;
          text-align: left;
          padding-right: 10px;
          span{
            font-size: 50px;
            color: white;
            font-weight: 200;
          }
        }
    }
    .text-bottom-left{
          display: flex;
          flex-direction: column;
          justify-content: end;          
        }

    /* inizio sesta parte del main */

     /* inizio settima parte main statica */
      
     .img-left{
       width: 50%;
       float: left;
       button{
         color: $colorTitolo;
         background-color: white;
         border: 1px solid white;
         border-radius: 5px;
         padding: 5px 10px;
       }
       p{
         color: $colorParagrafi;
         font-size: 13px;         
       }
     }
     span{
        font-size: 10px;
        color: $colorParagrafi;
        font-weight: bold;        
      }
     .img-right{
       width: 50%;
       float: left;
        button{
          color: $colorTitolo;
          background-color: white;
          border: 1px solid white;
          border-radius: 5px;
          padding: 5px 10px;
        }
        p{
         color: $colorParagrafi;
         font-size: 13px;         
       }
       span{
        font-size: 10px;
        color: $colorParagrafi;
        font-weight: bold;        
      }
     }
     /* fine settima parte main statica */
     /* inizio ottava parte main statico */

     .ms_float-23{
       float: left;
       width: calc(100% / 4 - 20px);
       margin: 0px 10px;
     }
     .ms_float-46{
       width: calc(100% / 2 - 20px);
       margin: 0px 10px;
       float: left;
       background-color: rgb(238, 231, 231);
       height: 96%;
       button{
              padding: 5px 15px;
              background-color: $colorTitolo;
              border: 1px solid white;
              border-radius: 8px;
              font-size: 20px;
              color: white;  
      }
     }
     .img-top-part{
       height: 250px;
       span{
        font-size: 10px;
        color: $colorParagrafi;
        font-weight: bold;        
      }
     }

     /* fine ottava parte main statico */
     /* inizio nona parte main statico */
     /* fine nona parte main statico */

   /* inizio generale del main */

  .ms_container::after{
    clear: both;
    content: '';
    display: table;
  }
  .ms_container-third::after{
    clear: both;
    content: '';
    display: table;
  }
  .ms_container-80{
    width: 80%;
    height: 500px;
    margin: 0 auto;
  }
  .ms_container-80-2{
    width: 80%;
    margin: 0 auto;
  }
  .background-img-bread{
    background-image: url('../assets/pexels-karolina-grabowska-4495761.jpg');
    background-size: cover;
  }
  .background-img-bread-2{
    background-image: url('../assets/pexels-pixabay-209196.jpg');
    background-size: cover;
    background-position-y: -7em;
  }
  .background-img-bread-3{
    background-image: url('../assets/pexels-marta-dzedyshko-7693958.jpg');
    background-size: cover;
    background-position: bottom;
    height: 400px;
  }
  .ms_background-grey{
      background-color: rgb(238, 231, 231);
  }
  .ms_background-yellow{
    background-color: rgba(235, 235, 159, 0.5);
  }
  .ms_style-h{
  color: $colorTitolo;
  font-size: 27px;
  font-weight: bold;
 }
 .ms_button-white{
   padding: 5px 15px;
   background-color: white;
   border: 1px solid white;
   border-radius: 8px;
   font-size: 15px;
   color: $colorTitolo;     
 }
</style>