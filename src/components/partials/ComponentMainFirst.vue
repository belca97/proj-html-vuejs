<template>
   <div class="container ms_container">
     
          <div class="text-first-part p-3">
            <span>OUR PRODUCT</span>
            <p>All our delectable pastries are backed fresh in our Kitchen very morning, and are made with all-natural, all organic ingredients</p>
            <button>Star shopping</button>

          </div>
          <div class="img-center-first-part">
            <img v-for="(thumb, index) in thumbsOne" :key="index" :src="(thumb.thumb)" alt="">
            <div class="ms_prev">
              <i class="fas fa-angle-left"></i>
            </div>
          </div>
          <div class="img-right-first-part">
              <img v-for="(thumb, index) in thumbsTwo" :key="index" :src="(thumb.thumb)"  alt="">
              <div class="ms_next">
                <i class="fas fa-angle-right"></i>
              </div>
          </div>

    </div>
</template>

<script>
export default {
  name: 'ComponentMainFirst',
  data(){
    return{
      thumbsOne:[
        {
          thumb : require('/src/assets/pexels-diana-akhmetianova-7296682.jpg')
        }
      ],
      thumbsTwo :[
        {
          thumb : require('/src/assets/pexels-diana-akhmetianova-7296683.jpg')
        }
      ]
    }
  }
}
</script>

<style scoped lang='scss'>
@import 'src/assets/variabili.scss';
      /*inzio prima parte del main in maniera statica */
    .text-first-part{
        float: left;
        width: calc(100% / 3 - 30px);
        height: 400px;
        button{
             padding: 10px 32px;
             background-color: $colorTitolo;
             border: 1px solid white;
             border-radius: 8px;
             font-size: 20px;
             color: white;          
        }
        p{
          color: $colorTitolo;
          font-size: 30px;
          margin: 40px 0px;
        }
        span{
          color: $colorTitolo;
          font-size: 10px;
        }
    }
    .img-center-first-part{
        float: left;
        width: calc(100% / 3 - 10px);
        height: 600px;
        position: relative;
        img{
          width: 100%;
          height: 100%;
          object-fit: cover;
        }
        .ms_prev{
          position: absolute;
          top: 45%;
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
    .img-right-first-part{
        float: right;
        width: calc(100% / 3 - 10px);
        height: 600px;
        position: relative;
        img{
          width: 100%;
          height: 100%;
          object-fit: cover;
        }
        .ms_next{
          position: absolute;
          top: 45%;
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
    }
          /*fine prima parte del main in maniera statica */
</style>