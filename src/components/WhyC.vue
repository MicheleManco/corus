<template>
  <div>
    <div class="container-fluid ">
      <div class="row">
        <h1 class="col-12 text-center why-cinese clr-gray"><strong> PERCHE FREQUENTARE UN <span class="clr-red">CORSO DI CINESE</span>?</strong> </h1>

        <div class="col-md-4 d-none d-xl-block position-relative">
          <img class="image" src="../assets/prima-immagine.jpg" alt="">
        </div>

        <div class="col-xl-4 col-sm-6 paragrafi">
          <p class="clr-gray-dark fs-5"> i sempre più frequenti scambi commerciali e culturali con la Cina hanno fatto sì che il Cinese sia divenuto in pochi anni una delle lingue più studiate a livello mondiale nonché un importante strumento di lavoro e di scambio culturale.</p>
          <h4 class="clr-gray fs-3"><strong><span class="clr-red ">QUALE CINESE</span>  INSEGNAMO?</strong></h4>
          <p class="clr-gray-dark fs-5" >Il corso propone l'insegnamento del Putonghua (普通話), altrimenti detto <strong>Mandarino</strong>, ossia la <strong> lingua ufficiale adottata dalla Repubblica Popolare Cinese</strong>, del relativo sistema di trascrizione fonetica Pīnyīn e delle regole di scrittura caratteri.</p>
        </div>

        <div class="col-xl-4 col-sm-6 bg-lightgray clr-gray">
          <div>
            <h4 class="fs-3 coordinate"><strong>COORDINATE</strong></h4>

            <div class="d-flex">
              <div class="images">
                <img src="../assets/orologio.png" alt="">
              </div>
              <div>
                <h5 class="clr-red fs-4"><strong>Durata</strong></h5>
                <p class="fs-5">Ottobre - maggio per un totale di 60 ore</p>
              </div>
            </div>

            <div class="d-flex">
              <div class="images">
                <img src="../assets/posizione.png" alt="">
              </div>
              <div>
                <h5 class="clr-red fs-4"><strong>Sede</strong></h5>
                <p class="fs-5">Il corso si terrà presso la sede di Corus s.a.s. in Via Lautelmonte, 32 a Esine(Brescia)</p>
              </div>
            </div>

            <div class="d-flex">
              <div class="images">
                <img src="../assets/people.png" alt="">
              </div>
              <div>
                <h5 class="clr-red fs-4"><strong>ORGANIZZAZIONE</strong></h5>
                <p class="fs-5">Gli allievi verranno organizzati in gruppi di massimo 5 persone</p>
              </div>
            </div>

            <div class="d-flex">
              <div class="images">
                <img src="../assets/attestato-icon.png" alt="">
              </div>
              <div>
                <h5 class="clr-red fs-4"><strong>ATTESTATO DI PARTECIPAZIONE</strong></h5>
              </div>
            </div>
          </div>

        </div>
      </div>
    </div>

    <!-- striscia rossa  -->
    <div class="bg-red">
      <div class="container">
        <div class="row justify-content-center d-flex text-center">
          <div class="col-12 col-md-6">
            <div class="fs-4">L'allievo può scegliere tra <span class="robotoB">2 livelli di apprendimento</span> in base alle conoscenze della lingua già acquisite.</div>
          </div>
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'WhyC',
  props: {
   
  }
}
</script>

<style scoped lang="scss">
.robotoB{
   font-family: 'Roboto';
   font-weight: 700;
}
.coordinate{
  margin-bottom: 20px;
}
.fs-5{
  line-height: 25px;
}
.clr-gray-dark{
  color: #3a3a3a;
}
.clr-gray{
  color: #535353;
}

.bg-red{
  background-color: #ba122b;
  color: white;
  font-size: 22px;
  line-height: 23px;
  padding: 22px;
  margin: 60px 0 10px 0;
}
.why-cinese{
  margin: 40px 0;
}

.paragrafi{
  padding: 20px 45px 20px 45px;
}
.images{
  margin-right: 15px;
}
.bg-lightgray{
  background-color: #e5e5e5;
  padding: 20px 200px 20px 20px;
}
.image{
  position: absolute;
  right: 0;
  height: 100%;
}
@media all and (max-width: 575px){
.why-cinese{
  margin: 40px 0 0 0;
}
}
@media all and (max-width: 1200px){
.bg-lightgray{
  padding: 20px 190px 20px 20px;
}
}
@media all and (max-width: 900px){
.bg-lightgray{
  padding: 20px 90px 20px 20px;
}
}
@media all and (max-width: 400px){
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