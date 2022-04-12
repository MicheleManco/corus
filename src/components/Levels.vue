<template>
  <div>
      <div class="container">
          <div class="row">
            <div class="col-12 livelli">
                <h4 class="clr-red"> <strong>2 LIVELLI DI APPRENDIMENTO</strong></h4>
                <div class="sottotitolo-levels" ><strong>le competenze acquisibili con i corsi di cinese e giapponese in aula</strong></div>
            </div>
        </div>
      </div>
      
    <!-- card di informazione corsi -->
    <div class="container">
        <div class="row">

            <div v-for="corso,i in corsi" :key="i" class="col-md-6 col-12 position-relative margine-card">
                <div class="d-flex">
                    <img class="pallino-corso d-none d-sm-block" :src="require('../' + corso.image)" alt="">
                    <div class="info-card">
                        <h5 class="clr-red titoletto"><strong>{{corso.title}}</strong></h5>
                        <p>{{corso.text}}</p>
                        <div class="position-absolute bottom-0 start-20 position-relative">
                            {{corso.comment}}
                            <!-- <div class="sfondo-gray"></div> -->
                        </div>
                    </div>
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
                <h4 class="clr-red"><strong>ATTESTATO DI PARTECIPAZIONE</strong></h4>
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
                    <div class="contattaci"><strong>Contattaci per ricevere tutti i dettagli dei</strong></div> 
                    <h4 class="clr-red"><strong>CORSI DI LINGUA CINESE E GIAPPONESE IN AULA</strong></h4>
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
.livelli{
    margin: 30px 0 40px 0;
    .sottotitolo-levels{
        font-size: 25px;
        line-height: 25px;
        color: #4c4c4c;
    }
}

.margine-card{
    margin-bottom: 50px;
}

.bg-lightgray{
    background-color: rgb(235, 235, 235);
    padding: 20px 0;
}
.info-card{
    padding-bottom: 100px;
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
</style>
