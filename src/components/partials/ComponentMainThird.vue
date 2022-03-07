<template>
<div class="container my-5">
          <div class="ms_container-third">
              <div class="text-third-part text-center d-flex flex-column justify-content-center  align-items-center">
                <span class="pb-3">Find a freshly baked product perfect for you</span>
                <p>Integer a nibh vitae ex porttitor rutrum <br> et ut velit. Etiam ac felis at leo feugat placerat. Sed ac nulla id orci tempor convallis sed</p>
                <button>Shop All Product</button>
              </div>
              <div class="img-third-part" v-for="(thumb, index) in thumbsOne" :key="index">
                <img class="w-100" :src="(thumb.thumb)" alt="">
                  <div class="ms_prev">
                      <i class="fas fa-angle-left"></i>
                  </div>
                  <div class="text-center pt-2">
                    <p>{{thumb.product}}</p>
                    <span>{{thumb.price}}</span>
                  </div>                
              </div>

              <div class="img-third-part" v-for="(thumb, index) in thumbsTwo" :key="index">
                <img class="w-100" :src="(thumb.thumb)"  alt="">
                <div class="text-center pt-2">
                    <p>{{thumb.product}}</p>
                    <span>{{thumb.price}}</span>
                </div>       
              </div>
              
              <div class="img-third-part" v-for="(thumb, index) in thumbsThird" :key="index">
                <img class="w-100" :src="(thumb.thumb)"  alt="">
                <div class="text-center pt-2">
                    <p>{{thumb.product}}</p>
                    <span>{{thumb.price}}</span>
                 </div>       
              </div>
              
              <div class="img-third-part" v-for="(thumb, index) in thumbsFourth" :key="index">
                <img class="w-100" :src="(thumb.thumb)"  alt="">
                    <div class="ms_next">
                        <i class="fas fa-angle-right"></i>
                    </div> 
                    <div class="text-center pt-2">
                      <p>{{thumb.product}}</p>
                    <span>{{thumb.price}}</span>
                  </div>      
              </div>
          </div>
      </div>  
</template>

<script>
export default {
    name : 'ComponentMainThird',
    data(){
    return{
      thumbsOne:[
        {
          thumb : require('/src/assets/img-terza-parte/pexels-clem-onojeghuo-375904.jpg'),
          product : 'A Lot Of Cookies',
          price : '$19.00-$39.00'          
        }
      ],
      thumbsTwo :[
        {
          thumb : require('/src/assets/img-terza-parte/pexels-ylanite-koppens-2014693.jpg'),
          product : 'Perfect Macarons',
          price : '$24.00-$62.00'
        },
      ],
      thumbsThird:[
        {
          thumb : require('/src/assets/img-terza-parte/pexels-pixabay-269235.jpg'),
          product : 'Strawberry Donut',
          price : '$24.00-$42.00'
        }
      ],
      thumbsFourth :[
        {
          thumb : require('/src/assets/img-terza-parte/pexels-istvan-szabo-10338830.jpg'),
          product : 'Heart Biscuits',
          price : '$24.00-$62.00'
        },
      ]
    }
  }
}
</script>

<style scoped lang='scss'>
@import 'src/assets/variabili.scss';
    /*inizio terza parte del main in maniera statica */
.ms_container-third{
      height: 400px;
    }
    .text-third-part{
      width: 28%;
      float: left;
      height: 80%;
      padding: 20px;
        button{
             padding: 5px 15px;
             background-color: $colorTitolo;
             border: 1px solid white;
             border-radius: 8px;
             font-size: 20px;
             color: white;   
        }
        p{
          color: $colorParagrafi;
        }
        span{
          color: $colorTitolo;
          font-weight: bold;
          font-size: 30px;
        }
    }
    .img-third-part{
      width: calc(72% / 4 - 16px);
      float: left;
      height: 100%;
      margin: 0px 8px;
      position: relative;
      p{
        font-weight: bold;
        color: $colorTitolo;
      }
      img{
        object-fit: cover;
        object-position: -5rem;
        height: 80%;
      }
      .ms_next{
          position: absolute;
          top: 35%;
          right: 0%;
          background-color: $colorParagrafi;   
          width: 35px;
          height: 60px;
          color: white;
          font-size: 20px;
          display: flex;
          justify-content: center;
          align-items: center;          
        }
        .ms_prev{
          position: absolute;
          top: 35%;
          background-color: $colorParagrafi;   
          width: 35px;
          height: 60px;
          color: white;
          font-size: 20px;
          display: flex;
          justify-content: center;
          align-items: center;
        }         
    }
    span{
        font-size: 10px;
        color: $colorParagrafi;
        font-weight: bold;        
      }
        /*fine terza parte del main in maniera statica */

</style>