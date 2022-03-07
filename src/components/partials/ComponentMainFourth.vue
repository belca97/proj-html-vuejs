<template>
<!-- Quarta Parte Main -->
<div class="ms_container-80 background-img-bread mb-3 mt-5 p-5">
            <div class="top-text-01">
              <div class="text-left">
                <p>Tell us what you have in <br> ming</p>
              </div>
              <div class="text-right">
                <span>01</span>
              </div>
            </div>
            <div class="text-bottom-right pt-5">
              <span class="pb-4">MANUAL INGREDIENT SELECTION</span>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur quam eius qui iure corporis placeat nesciunt dicta minima, 
                ducimus et quisquam recusandae doloribus atque praesentium at ipsam inventore iste optio.
                ducimus et quisquam recusandae doloribus atque praesentium at ipsam inventore iste optio.
                ducimus et quisquam recusandae doloribus atque praesentium at ipsam inventore iste optio.
                ducimus et quisquam recusandae doloribus atque praesentium at ipsam inventore iste optio.</p>
            </div>      

        </div> 
</template>

<script>
export default {
    name : 'ComponentMainFourth'
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
    .text-bottom-right{
      width: 50%;
      float: right;
      display: flex;
      flex-direction: column;
      justify-content: center;
      height: 80%;
      span{
        font-size: 13px;
        color: $colorParagrafi;
        font-weight: bold;
      }
      p{
        color: white;
        font-weight: bold 700;
      }
    }
  .background-img-bread{
    background-image: url('/src/assets/pexels-karolina-grabowska-4495761.jpg');
    background-size: cover;
  }
</style>