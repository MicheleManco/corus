<template>
  <div>
    <div class="bg-light-gray1 fs-5">
      <div class="container">
        <div class="row">
          <div class="col-sm-6 d-none d-lg-flex d-flex justify-content-end">
              <img class="women-img" src="../assets/women.png" alt="">
          </div>
          <div class="col-lg-5 col-12 d-flex flex-column justify-content-center container-text">
              <div class="clr-red fs-3 robotoB">DOCENTI QUALIFICATI</div>
              <div class="fs-3 clr-gray robotoB">per corsi di cinese</div>
              <div class="fs-3 sottotitoletto clr-gray robotoB"> e giapponese davvero efficaci</div>
            <p class="clr-gray-dark ">I nostri docenti sono tutti accuratamente selezionati e hanno maturato molti anni di esperienza nell'insegnamento della lingua e della cultura cinese/giapponese e presso scuole medie e superiori, aziende, centri linguistici  e associazioni culturali.</p>
          </div>
        </div>
      </div>
    </div>
    

    <div class="bg-light-gray2 fs-5">
      <div class="container">
        <div class="row">
          <div class="col-md-7 col-12 clr-gray-dark">
            <p>Corus s.a.s. raggruppa un <span class="robotoB">team di traduttori e interpreti professionisti specializzati nelle Lingue Orientali</span>: Cinese, Giapponese e Coreano </p>
            <div>Oltre ai corsi di lingua cinese e giapponese, Corus offre anche servizi di traduzione e interpretariato, asseverazione, legalizzazione e impaginazione grafica nelle principali Lingue Orientali</div>
          </div>
          <div class="col-md-5 gy-3  d-flex flex-column justify-content-center align-items-center">
            <img class="logo" src="../assets/logo.png" alt="">
          </div>
        </div>
      </div>
    </div>
      
      
  </div>
</template>

<script>
export default {
  name: 'Info',
  props: {
   
  }
}
</script>

<style scoped lang="scss">
.fs-3{
  line-height: 30px;
}
.robotoB{
   font-family: 'Roboto';
   font-weight: 700;
}
.fs-5{
  line-height: 25px;
}
.clr-gray-dark{
  color: #3a3a3a;
}
.clr-gray{
  color: #4c4c4c;
}
.container-text{
  margin: 45px 0;
}
.bg-light-gray1{
  background-color: #e5e5e5;
  margin-top: 155px;
  img{
    margin-top: -90px;
    margin-right: 30px;
  }
}
.bg-light-gray2{
  background-color: #f5f5f5;
  margin: 25px 0;
  padding: 35px 0;
  img{
    width: 300px;
  }
}
.sottotitoletto{
  margin-bottom: 30px;
}

@media all and (max-width: 390px){
   .logo{
     max-width: 80%;
   }
}
@media all and (max-width: 1200px){
   .bg-light-gray1{
  background-color: #e5e5e5;
  margin-top: 155px;
  img{
    margin-top: 10px;
    margin-right: 50px;
  }
}
}
</style>