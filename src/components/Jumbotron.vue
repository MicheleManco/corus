<template>
  <div class="big-container">
    <div class="container">
      <div class="row core">

        <div class="col-9 row ">
          <div class="col-4"> <!--spaziatore --></div>

          <div class="row col-8 debug3">
            <div class="col-12 spazio-titolo-top"></div>
            <div class="col-12"><h1>Corsi di Lingua Cinese e Giapponese</h1></div>

            <div class="col-12 row">
              <div class="col-3"></div>
              <div class="col-9">
                <div>corsi in aula a Brescia</div>
                <div><img src="../assets/check-yellow.png" alt=""><strong>2 livelli di apprendimento (A1 e A2)</strong></div>
                <div><img src="../assets/check-yellow.png" alt=""><strong>docenti qualificati</strong></div>
                <div><img src="../assets/check-yellow.png" alt=""><strong>attestato di partecipazione</strong> rilasciato al termine del corso</div>
              </div>
            </div>
          </div>

          <div class="col-12 bg-gray">
            <h4>PARTECIPA AI CORSI IN AULA</h4>
            <div>e apprendi la lingua cinese e giapponede da docenti qualificati</div>
            <div>termine iscrizioni 7 Ottobre</div>
          </div>

        </div>

        <!-- form------------------------------------------------------------------------- -->
        <div class="col-3 bg-light-black">
          
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

          <div class="invia_richiesta"><div>Invia Richiesta</div><img src="../assets/arrow-right.png" alt=""></div>

        </div>
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
  background-size: 100%;
  background-position: top;
  padding-top: 80px;
}
.spazio-titolo-top{
  height: 30px;
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
.bg-gray{
  margin-top: 120px;
  background-color: gray;
  height: 100px;
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
// debug------------------------------------------------------


.debug3{
  background-color: purple;
}
</style>
