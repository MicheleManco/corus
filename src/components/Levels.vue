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
    <div class="container-fluid ">
        <div class="row container-card">

            <div v-for="corso,i in corsi" :key="i" class="col-md-6 col-12 position-relative margine-card">
                <div class="d-flex content">
                    <img class="pallino-corso d-none d-sm-block" :src="require('../' + corso.image)" alt="">
                    <div class="info-card">
                        <h5 class="clr-red titoletto robotoB fs-4">{{corso.title}}</h5>
                        <p>{{corso.text}}</p>
                    </div>
                </div>
                <div class="position-absolute bottom-0 start-20 position-relative commento robotoB">
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
                    <div class="contattaci robotoB fs-3">Contattaci per ricevere tutti i dettagli dei</div> 
                    <div class="clr-red robotoB fs-3">CORSI DI LINGUA CINESE E GIAPPONESE IN AULA</div>
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
.container-card{
    margin-bottom: -20px;
}
.fs-3{
    line-height: 30px;
}
.robotoB{
   font-family: 'Roboto';
   font-weight: 700;
}

.livelli{
    margin: 60px 0 40px 0;
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
    color: #4f4f4f;
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
    margin-bottom: 25px;
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
    margin-bottom: 30px;
    img{
        margin-right: 35px;
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
@media all and (max-width: 1530px){
    .info-card{
    padding-bottom: 50%;
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
    .margine-card:nth-child(1) .commento,.margine-card:nth-child(2) .commento{
        height: 20%;
    }
    .margine-card:nth-child(3) .commento,.margine-card:nth-child(4) .commento{
        height: 27%;
    }
    .info-card{
        padding-bottom: 60%;
    }
}
@media all and (max-width: 1080px){
    .info-card{
        padding-bottom: 50%;
    }
    .info-card{
        padding-bottom: 70%;
    }
    .margine-card:nth-child(1) .commento,.margine-card:nth-child(2) .commento{
        height: 20%;
    }
}
@media all and (max-width: 915px){
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
    .margine-card:nth-child(3) .commento,.margine-card:nth-child(4) .commento{
        padding:10px 50px 10px  16%;  
        right: 0;
        height: 23%;
    }
    .info-card{
        padding-bottom: 66%;
    }
}
@media all and (max-width: 767px){
    .info-card{
        padding-bottom: 30%;
    }
    .margine-card:nth-child(1) .commento,.margine-card:nth-child(2) .commento,.margine-card:nth-child(4) .commento{
        padding:10px;
        height: 25%;
    }
    .margine-card:nth-child(3) .commento{
        height: 35%;
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
    }
}
@media all and (max-width:630px){
    .info-card{
        padding-bottom: 30%;
    }
    .margine-card:nth-child(1) .commento,.margine-card:nth-child(2) .commento,.margine-card:nth-child(4) .commento{
        padding-left:80px;
        height: 25%;
    }
    .margine-card:nth-child(3) .commento{
        height: 35%;
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
        height: 20%;
    }
    .margine-card:nth-child(1) .commento{
        padding:10px;  
        right: 0;
        height: 25%;
    }
    .margine-card:nth-child(3) .commento{
        height: 30%;
        padding: 10px;
    }
    .info-card{
        padding-bottom: 50%;
    }
}
@media all and (max-width:391px){
    .margine-card:nth-child(4) .commento,.margine-card:nth-child(1) .commento,.margine-card:nth-child(2) .commento{
        height: 20%;
    }
    .margine-card:nth-child(3) .commento{
        height: 30%;
    }
    .info-card{
        padding-bottom: 80%;
    } 
}
@media all and (max-width:298px){
    .info-card{
        padding-bottom: 100%;
    }
}
</style>
