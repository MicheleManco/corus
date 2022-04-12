<template>
  <div>
    <div class="bg-light-gray1">
      <div class="container">
        <div class="row">
          <div class="col-sm-6 d-none d-lg-flex d-flex justify-content-end">
              <img class="women-img" src="../assets/women.png" alt="">
          </div>
          <div class="col-lg-5 col-12 d-flex flex-column justify-content-center">
            <h3 class="clr-red"><strong>DOCENTI QUALIFICATI</strong></h3>
            <h3 class="sottotitoletto clr-gray"><strong>per corsi di cinese e giapponese davvero efficaci</strong></h3>
            <p class="clr-gray-dark">i nostri docenti sono tutti accuratamente selezionati e hanno maturato molti anni di esperienza nell'inseguimento della lingua e della cultura cinese/giapponese e presso scuole medie e superiori, aziende, centrii linguistici  e associazioni culturali.</p>
          </div>
        </div>
      </div>
    </div>
    

    <div class="bg-light-gray2">
      <div class="container">
        <div class="row">
          <div class="col-md-7 col-12 clr-gray-dark">
            <p>Corus s.a.s. raggruppa un <span><strong>team di traduttori e interpreti professionisti specializzati nelle Lingue Orientali</strong></span>: Cinese,Giapponese e Coreano </p>
            <p>Oltre ai corsi di lingua cinese e giapponese, Corus offre anche servizi di traduzione e interpretariato, asseverazione, legalizzazione e impaginazione grafica nelle principali Lingue Orientali</p>
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
.clr-gray-dark{
  color: #3a3a3a;
}
.clr-gray{
  color: #4c4c4c;
}
.bg-light-gray1{
  background-color: #e5e5e5;
  img{
    margin-top: -70px;
    margin-right: 50px;
  }
}
.bg-light-gray2{
  background-color: #f5f5f5;
  margin: 25px 0;
  padding: 25px 0;
  img{
    width: 300px;
  }
}
.sottotitoletto{
  margin: -10px 0 30px 0;
}

@media all and (max-width: 390px){
   .logo{
     max-width: 80%;
   }
}
</style>