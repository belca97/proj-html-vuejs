<template>
<div class="ms_container-80 ms_container mb-3">
            <div class="img-left-quinta-parte background-img-bread-3 h-100 p-5">
                <div class="top-text-01">
                  <div class="text-left">
                    <p>We Start Baking</p>
                  </div>
                  <div class="text-right">
                    <span>02</span>
                  </div>
               </div>
                <div class="text-bottom-left w-50">
                  <span class="pb-3">SWEET & DELICIOUS</span>
                  <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Qui dolorem nam quas autem nesciunt molestias cumque itaque illum corrupti odio aliquid quam atque, unde veritatis laborum dolore suscipit recusandae porro?</p>
                </div>
            </div>
            <div class="testo-right-quinta-parte h-100 p-5">
              <div class="h-100 d-flex  flex-column justify-content-center px-5">
                <span class="pb-5">DONT JUST TAKE OUR WORD FOR IT</span>
                <p>"Fynally found an alternative to the mass produced products. Somethings that incorporates real organic ingredients, nutrient dense 
                  wellness while promoting sustainability and activity"</p>
                <span class="pt-5">Rachel Cooper, Founder</span>
              </div>
            </div>
</div>  
</template>

<script>
export default {
    name :'ComponentMainFifth'
}
</script>

<style scoped lang='scss'>
@import 'src/assets/variabili.scss';
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
.img-left-quinta-parte{
      float: left;
      width: 49%;
      height: 90%;
    }
    .text-bottom-left{
      height: 80%;
      display: flex;
      justify-content: flex-end;
      flex-direction: column;

      p{
        color: white;
        font-weight: bold 700;        
      }
    }
     span{
        font-size: 10px;
        color: $colorParagrafi;
        font-weight: bold;        
      }

    .testo-right-quinta-parte{
      float: right;
      width: 49%;
      height: 90%;
      background-color: rgb(238, 231, 231);
      p{
        color: $colorTitolo;
        font-size: 27px;
        font-weight: bold;
      }
    }
    .background-img-bread-3{
            background-image: url('/src/assets/pexels-marta-dzedyshko-7693958.jpg');
            background-size: cover;
            background-position: bottom;
            height: 400px;
    }
</style>