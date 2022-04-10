<template>
  <div>
      <div class="container">
          <div class="row">
            <div class="col-12">
                <h2 class="clr-red">2 LIVELLI DI APPRENDIMENTO</h2>
                <p>le competenze acquisibili con i corsi di cinese e giapponese in aula</p>
            </div>
        </div>
      </div>
      
    <!-- card di informazione corsi -->
    <div class="container">
        <div class="row">

            <div v-for="corso,i in corsi" :key="i" class="col-md-6 col-12 position-relative ">
                <div class="d-flex">
                    <img class="pallino-corso d-none d-sm-block" :src="require('../' + corso.image)" alt="">
                    <div class="info-card">
                        <h5 class="clr-red titoletto">{{corso.title}}</h5>
                        <p>{{corso.text}}</p>
                         <p class="position-absolute bottom-0 start-20 bg-gray">{{corso.comment}}</p>  <!--position absolute per farlo stare sotto -->
                    </div>
                </div>
                
                
            </div>

        </div>
    </div>

    <!-- sezione attestato di partecipazione-->
    <div class="container">
        <div class="row attestato">
            <div class="col-sm-4 d-none d-sm-flex col-12 d-flex justify-content-end ">
                <img src="../assets/attestato.jpg" alt="">
            </div>
            <div class="col-sm-8 col-12 d-flex flex-column justify-content-center">
                al termine di ogni corso, tutti i partecipanti riceveranno un
                <h4 class="clr-red"><strong>ATTESTATO DI PARTECIPAZIONE</strong></h4>
            </div>
        </div>
    </div>

    <div class="bg-lightgray">
        <div class="container">
            <div class="row ">
                <div class="col-sm-4 d-none d-sm-flex col-0  justify-content-end">
                    <img src="../assets/arrow-pallino.png" alt="">
                </div>
                <div class="col-sm-8 col-12 d-flex flex-column justify-content-center">
                    <strong>Contattaci per ricevere tutti i dettagli dei</strong> 
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
.pallino-corso{
    height: 50px;
    margin-right: 15px;
}
.attestato{
    margin: 30px 0;
}
</style>
