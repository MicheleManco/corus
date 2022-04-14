<template>
  <div class="fs-5">
      <div class="container">
          <div class="row">
            <div class="col-12 livelli">
                <h4 class="clr-red robotoB fs-2"> 2 LIVELLI DI APPRENDIMENTO</h4>
                <div class="sottotitolo-levels robotoB fs-3" >le competenze acquisibili con i corsi di cinese e giapponese in aula</div>
            </div>
        </div>
      </div>
      
    <!-- card di informazione corsi -->
    <div class="container-fluid">
        <div class="row container-card">

            <div v-for="corso,i in corsi" :key="i" class="col-md-6 col-12 position-relative margine-card">
                <div class="d-flex content">
                    <img class="pallino-corso d-none d-sm-block" :src="require('../' + corso.image)" alt="">
                    <div class="info-card">
                        <h5 class="clr-red titoletto robotoB fs-4">{{corso.title}}</h5>
                        <p>{{corso.text}}</p>
                    </div>
                </div>
                <div class="position-absolute bottom-0 start-20 position-relative commento">
                    {{corso.comment}}
                </div>
            </div>

        </div>
    </div>

    <!-- sezione attestato di partecipazione-->
    <div class="container">
        <div class="row attestato">
            <div class="col-sm-4 d-none d-sm-flex d-flex justify-content-end ">
                <img src="../assets/attestato.jpg" alt="">
            </div>
            <div class="col-sm-8 col-12 d-flex flex-column justify-content-center">
                <div class="al-termine">Al termine di ogni corso, tutti i partecipanti riceveranno un</div>
                <h4 class="clr-red robotoB">ATTESTATO DI PARTECIPAZIONE</h4>
            </div>
        </div>
    </div>

    <div class="bg-lightgray">
        <div class="container">
            <div class="row last-row">
                <div class="col-sm-4 d-none d-sm-flex justify-content-end">
                    <img src="../assets/arrow-pallino.png" alt="">
                </div>
                <div class="col-sm-8 col-12 d-flex flex-column justify-content-center">
                    <div class="contattaci robotoB">Contattaci per ricevere tutti i dettagli dei</div> 
                    <h4 class="clr-red robotoB">CORSI DI LINGUA CINESE E GIAPPONESE IN AULA</h4>
                </div>
                <div class="d-sm-none ">
                    <img src="../assets/arrow-pallino.png" alt="">
                </div>
            </div>
        </div>
    </div>


  </div>
</template>

<script>
export default {
  name: 'Levels',
  props: {
   corsi:Array,
  }
}
</script>

<style scoped lang="scss">
.robotoB{
   font-family: 'Roboto';
   font-weight: 700;
}
.livelli{
    margin: 30px 0 40px 0;
    .sottotitolo-levels{
        font-size: 25px;
        line-height: 25px;
        color: #4c4c4c;
    }
}
.margine-card:nth-child(2) .content,.margine-card:nth-child(4) .content{
    padding-right: 30%;
}
.margine-card:nth-child(1) .content,.margine-card:nth-child(3) .content{
    padding-left: 30%;
}
.margine-card:nth-child(2) .commento,.margine-card:nth-child(4) .commento{
    padding:10px 30% 10px 50px;
}
.margine-card:nth-child(1) .commento,.margine-card:nth-child(3) .commento{
    padding:10px 50px 10px  36%;  
    right: 0;
}

.commento{
    background-color: #dcdcdc;
    width: 100%;
    height: 23%;
}
.margine-card{
    margin-bottom: 50px;
}

.bg-lightgray{
    background-color: rgb(235, 235, 235);
    padding: 35px 0;
}
.info-card{
    padding-bottom: 30%;
}
.titoletto{
    line-height: 50px;
    vertical-align: center;
}
.al-termine{
    font-size: 25px;
    line-height: 25px;
    color: #4c4c4c;
}
.pallino-corso{
    height: 50px;
    margin-right: 15px;
}
.attestato{
    margin: 30px 0px;
    img{
        margin-right: 50px;
    }
    
}
.contattaci{
    font-size: 25px;
    line-height: 25px;
    color: #4c4c4c;
}
.last-row{
    img{
        max-height: 50px;
    }
}
@media all and (max-width: 390px){
   .info-card{
    padding-bottom: 180px;
} 
.margine-card{
    margin-bottom: 20px;
}
}
@media all and (max-width: 1285px){
   
    .margine-card:nth-child(2) .content,.margine-card:nth-child(4) .content{
        padding-right: 10%;
    }
    .margine-card:nth-child(1) .content,.margine-card:nth-child(3) .content{
        padding-left: 10%;
    }
    .margine-card:nth-child(2) .commento,.margine-card:nth-child(4) .commento{
        padding:10px 30% 10px 50px;
    }
    .margine-card:nth-child(1) .commento,.margine-card:nth-child(3) .commento{
        padding:10px 50px 10px  36%;  
        right: 0;
    }
    .commento{
    background-color: #dcdcdc;
    width: 100%;
    height: 28%;
}
}
@media all and (max-width: 1080px){
    .info-card{
        padding-bottom: 50%;
    }
}
@media all and (max-width: 905px){
    .margine-card:nth-child(2) .content,.margine-card:nth-child(4) .content{
        padding-right: 1%;
    }
    .margine-card:nth-child(1) .content,.margine-card:nth-child(3) .content{
        padding-left: 1%;
    }
    .margine-card:nth-child(2) .commento,.margine-card:nth-child(4) .commento{
        padding:10px 10% 10px 60px;
    }
    .margine-card:nth-child(1) .commento,.margine-card:nth-child(3) .commento{
        padding:10px 50px 10px  16%;  
        right: 0;
    }
    .commento{
        background-color: #dcdcdc;
        width: 100%;
        height: 23%;
    }
    .info-card{
        padding-bottom: 45%;
    }
}
@media all and (max-width: 767px){
    .info-card{
        padding-bottom: 20%;
    }
    .commento{
        height: 30%;
    }
    .margine-card:nth-child(2) .content,.margine-card:nth-child(4) .content{
        padding-right: 1%;
    }
    .margine-card:nth-child(1) .content,.margine-card:nth-child(3) .content{
        padding-left: 1%;
    }
    .margine-card:nth-child(2) .commento,.margine-card:nth-child(4) .commento{
        padding:10px 10% 10px 14%;
        margin-left: -12px;
    }
    .margine-card:nth-child(1) .commento,.margine-card:nth-child(3) .commento{
        padding:10px 10% 10px  14%;  
        right: 0;
    }
}
@media all and (max-width:630px){
    .info-card{
        padding-bottom: 30%;
    }
}
@media all and (max-width:575px){
    .margine-card:nth-child(2) .content,.margine-card:nth-child(4) .content{
        padding-right: 0;
    }
    .margine-card:nth-child(1) .content,.margine-card:nth-child(3) .content{
        padding-left: 0;
    }
    .margine-card:nth-child(2) .commento,.margine-card:nth-child(4) .commento{
        padding:10px;
    }
    .margine-card:nth-child(1) .commento,.margine-card:nth-child(3) .commento{
        padding:10px;  
        right: 0;
    }
    .commento{
        height: 30%;
    }
    .info-card{
        padding-bottom: 50%;
    }
}
@media all and (max-width:391px){
    .margine-card:nth-child(4) .commento,.margine-card:nth-child(1) .commento,.margine-card:nth-child(2) .commento{
        height: 20%;
    }
}
@media all and (max-width:391px){
   .info-card{
        padding-bottom: 60%;
    } 
}
@media all and (max-width:295px){
    .info-card{
        padding-bottom: 80%;
    }
}
</style>
