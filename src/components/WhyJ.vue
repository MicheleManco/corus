<template>
  <div>
    <div class="container-fluid">
      <div class="row justify-content-center mini-container">
        <h1 class="col-12 text-center why-giapponese  clr-gray"><strong>PERCHE FREQUENTARE UN <span class="clr-red">CORSO DI GIAPPONESE</span>?</strong></h1>

        <div class="col-xl-4 col-sm-6 bg-lightgray clr-gray">
          <div>
          <h4><strong>COORDINATE</strong></h4>

          <div class="d-flex">
            <div>
              <img class="images" src="../assets/orologio.png" alt="">
            </div>
            <div>
              <h5 class="clr-red"><strong>Durata</strong></h5>
              <p>Ottobre - maggio per un totale di 60 ore</p>
            </div>
          </div>

          <div class="d-flex">
            <div>
              <img class="images" src="../assets/posizione.png" alt="">
            </div>
            <div>
              <h5 class="clr-red"><strong>Sede</strong></h5>
              <p>Il corso si terrà presso la sede di Corus s.a.s. in Via Lautelmonte, 32 a Esine(Brescia)</p>
            </div>
          </div>

          <div class="d-flex">
            <div>
              <img class="images" src="../assets/people.png" alt="">
            </div>
            <div>
              <h5 class="clr-red"><strong>ORGANIZZAZIONE</strong></h5>
              <p>Gli allievi verranno organizzati in gruppi di massimo 5 persone</p>
            </div>
          </div>

          <div class="d-flex">
            <div>
              <img class="images" src="../assets/attestato-icon.png" alt="">
            </div>
            <div>
              <h5 class="clr-red"><strong>ATTESTATO DI PARTECIPAZIONE</strong></h5>
            </div>
          </div>
          </div>
        </div>

        <div class="col-xl-4 col-sm-6 paragrafi ">
          <p class="clr-gray-dark" >L'occidente è da sempre interessato alla realtà nipponica, per le sue enormi potenzialità, ma anche per la sua affascinante variegata cultura: anime e manga, templi e castelli, geishe e samurai sono lo sfondo di una società ipertecnologica e alla moda. E oggi chi conosce il giapponese rappresenta un'importante risorsa per le aziende italiane che si affacciano su questo mercato. </p>
          <h4 class="clr-gray"><strong><span class="clr-red">QUALE GIAPPONESE</span>  INSEGNAMO?</strong></h4>
          <p class="clr-gray-dark" >Il corso propone l'insegnamento della lingua <strong>giapponese moderna</strong>, con le sue forme di scrittura (katakana, hiragana, kenji).</p>
        </div>

        <div class="col-md-4 d-none d-xl-block position-relative">
          <img class="image" src="../assets/men.jpg" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'WhyJ',
  props: {
   
  }
}
</script>

<style scoped lang="scss">
.clr-gray-dark{
  color: #3a3a3a;
}
.clr-gray{
  color: #535353;
}
.mini-container{
  margin-bottom: 120px;
}

.why-giapponese{
  margin: 40px 0;
}
.paragrafi{
  padding: 20px 60px 0 60px;
}
.images{
  margin-right: 15px;
}
.bg-lightgray{
  background-color: #e5e5e5;
  padding: 20px 20px 20px 200px;
}
.image{
  position: absolute;
  left: 0;
  height: 100%;
}
@media all and (max-width: 1400px){
.bg-lightgray{
  padding: 20px  20px 20px 100px;
}
}

@media all and (max-width: 1200px){
.bg-lightgray{
  padding: 20px  20px 20px 150px;
}
.paragrafi{
  padding: 20px 20px 0 30px;
}
}
@media all and (max-width: 900px){
.bg-lightgray{
  padding: 20px 20px 20px 50px;
}
}
@media all and (max-width: 500px){
.bg-lightgray{
  padding: 20px 20px 20px 20px;
}
}
@media all and (max-width: 500px){
.bg-lightgray{
  padding: 10px;
}
}
</style>