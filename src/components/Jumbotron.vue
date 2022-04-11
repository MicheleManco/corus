<template>
  <div class="big-container">
    <div class="container">
      <div class="row core d-flex justify-content-center">         <!--da 992px devo cambiare i margini attraverso css e non BS -->

        <div class="col-sm-9 col-12 row d-flex ">

          <div class="col-4 d-none d-xl-block"> <!--spaziatore --></div>

          <div class="row col-12 col-xl-8">
            <div class="col-12 d-none d-xl-block spazio-titolo-top"></div>
            <div class="col-12">
              <div class="main-title"><strong>Corsi di Lingua</strong></div>
              <div class="main-title"><strong>Cinese e Giapponese</strong></div>
            </div>
            <div class="col-12 row">
              <div class="col-3 d-none d-lg-block"></div>
              <div class="col-lg-9 col-12">
                <div class="titolo-lista">corsi in aula a Brescia</div>

                <div class="clr-white d-flex">
                  <img src="../assets/check-yellow.png" alt="">
                  <div><strong>2 livelli di apprendimento (A1 e A2)</strong></div>
                </div>

                <div class="clr-white d-flex">
                  <img src="../assets/check-yellow.png" alt="">
                  <div><strong>docenti qualificati</strong></div>
                </div>

                <div class="clr-white d-flex">
                  <img src="../assets/check-yellow.png" alt="">
                  <div><strong>attestato di partecipazione</strong> rilasciato al termine del corso</div>
                </div>
    
              </div>
            </div>
          </div>

          <div class="col-12 d-none d-lg-flex bg-gray align-self-end justify-content-between align-items-center">
            <div>
              <div class="titoletto-giallo"><strong>PARTECIPA AI CORSI IN AULA</strong></div>
              <div class="sottotitolo-bianco"><strong>e apprendi la lingua cinese e giapponede da docenti qualificati</strong></div>
              <div class="white-text">termine iscrizioni 7 Ottobre</div>
            </div>
            <img id="arrow-white" src="../assets/arrow-wh-right.png" alt="">
          </div>

        </div>

        <!-- form------------------------------------------------------------------------- -->
        <form class="col-3 bg-light-black position-relative" action="">
        <div>
          
          <div class="colore-orange head-form d-flex align-items-center"><div class="da_ottobre">da ottobre 2018</div></div>

          <div class="padding-blocco richiedi_info"><strong>Richiedi informazioni</strong> </div>

          <div class="padding-blocco">Nome e Cognome*</div>
          <input class="margin-blocco" type="text">
          <div class="padding-blocco">telefono</div>
          <input class="margin-blocco" type="text">
          <div class="padding-blocco">E-mail*</div>
          <input class="margin-blocco" type="text">
          <div class="padding-blocco">Corso di interesse</div>
          <select class="margin-blocco" name="interesse">
            <option value="Cinese-Base"> Cinese Base</option>
            <option value="Cinese-Elementare"> Cinese Elementare</option>
            <option value="Giapponese-Base"> Giapponese Base</option>
            <option value="Giapponese-Elementare"> Giapponese Elementare</option>
          </select>
          <div class="padding-blocco">Messaggio*</div>
          <div><textarea class="margin-blocco" name=""></textarea></div>

          <div>
            <div class="padding-blocco">*campi obbligatori</div>
            <div class="checkbox-container"><input class="checkbox" type="checkbox" name="termini"><a href=""> Accettazione Tratt. Dati Personali</a></div>
            
          </div>

            <button class="invia_richiesta" type="submit"><div>Invia Richiesta<img src="../assets/arrow-right.png" alt=""></div></button>

        </div>
        </form>
        
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'jumbotron',
  props: {
   
  }
}
</script>

<style scoped lang="scss">
.big-container{
  background-image: url("../assets/jumbotron.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: top;
  padding-top: 80px;
}
.spazio-titolo-top{
  height: 30px;
}

.main-title{
  color: white;
  font-size: 50px;
  line-height: 50px;
  margin-left: 124px;
  margin-right: -10px;
}
.titolo-lista{
  color: white;
  font-size: 27px;
  margin: 50px 0px 20px 116px;
}
.clr-white{
  color: white;
  margin-left: 80px;
  margin-bottom: 30px;
  img{
    margin-right: 10px;
    width: 26px;
    height: 24px;
  }
}

.colore-orange {
  background-color: #dc8122;
  width: 240px;
}
.head-form{
  color: white;
  width: 240px;
  height: 43px;
  padding: 0 20px;
  .da_ottobre{
    font-size: 19px;
    margin-bottom: 2px;
    padding: 0;
  }
}
.checkbox{
  margin-left: 20px;
}
.padding-blocco{
  padding: 0 20px;
  margin-top: 6px;
}
.margin-blocco{
  margin: 0 20px;
  width: 200px;
}
.richiedi_info{
  font-size: 30px;
  line-height: 30px;
  margin: 15px 0;
}

.invia_richiesta{
  height: 85px;
  width: 240px;
  font-size: 19px;
  color: rgb(39, 39, 39);
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #dc8122;
  position: absolute;
  bottom: 0px;
  border: none;
  img{
    margin-left: 20px;
  }
}

.bg-light-black{
  background-color: rgba(0, 0, 0, 0.493);
  color: white;
  width: 240px;
  padding: 0;
}
.checkbox-container{
  margin: 10px 0;
}
a{
  font-size: 13px;
  color: white;
  line-height: 14px;
}
.bg-gray{
  margin-top: 120px;
  background-color: #313131;
  height: 85px;
  padding: 0px 30px;
}
#arrow-white{
  margin-right: 10px;
}
.titoletto-giallo{
  color: #dc8122;
  font-size: 23px;
  line-height: 25px;
}
.sottotitolo-bianco{
  color: white;
  font-size: 20px;
  line-height: 22px;
}
.white-text{
  color: white;
  font-size: 18px;
}

@media all and (max-width: 992px) {
.big-container{
  padding-top: 15px;
  padding-bottom: 20px;
}
.invia_richiesta{
  bottom: -20px;
}
.main-title{
  color: white;
  font-size: 50px;
  line-height: 50px;
  margin-left: 0;
  margin-right: -40px;
  font-size: 40px;
}
.titolo-lista{
  margin-left: 0px;
}
.clr-white{
  color: white;
  margin-left: 0px;
  margin-bottom: 30px;
  img{
    margin-right: 10px;
    width: 26px;
    height: 24px;
  }
}
.titolo-lista{
  color: white;
  font-size: 27px;
  margin: 50px 0px 20px;
}
}

</style>
