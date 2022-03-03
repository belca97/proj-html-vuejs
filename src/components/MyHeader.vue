<template>
    <header>
        <div class="ms_container">
            <div class="logo-headed">

            </div>
            <div class="menu-header">
                <ul>
                    <li v-for='(testo, index) in TestiHeader' :key="index"><a href="">{{testo.text}}</a></li>
                    <li><a href=""></a></li>
                </ul>

            </div>

        </div>

    </header>
</template>

<script>
export default {
    name:'MyHeader',
    data (){
        return{


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
    height: 500px;
    background-color: $colorJubmtronHeader;

            .ms_container{
                height: 100px;
                    .logo-header{
                        float: left;
                        width: 10%;
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
}
.ms-container::after{
    display: table;
    clear: both;
    content: '';
}
  a:hover{
       border-bottom: 2px solid $colorMenuHeader
 }


</style>