<template>
  <div>
    <div class="container">
      <div class="row">
        <h1 class="col-12 text-center why-cinese">PERCHE FREQUENTARE UN <span class="clr-red">CORSO DI CINESE</span> ?</h1>

        <div class="col-md-4 d-none d-lg-block position-relative">
          <img class="image" src="../assets/prima-immagine.jpg" alt="">
        </div>

        <div class="col-lg-4 col-sm-6">
          <p> i sempre più frequenti scambi commerciali e culturali con la Cina hanno fatto sì che il Cinese sia divenuto in pochi anni una delle lingue più studiate a livello mondiale nonché un importante strumento di lavoro e di scambio culturale.</p>
          <h4><span class="clr-red">QUALE CINESE</span>  INSEGNAMO?</h4>
          <p>Il corso propone l'insegnamento del Putonghua (普通話), altrimenti detto <strong>Mandarino</strong>, ossia la <strong> lingua ufficiale adottata dalla Repubblica Popolare Cinese</strong>, del relativo sistema di trascrizione fonetica Pīnyīn e delle regole di scrittura caratteri.</p>
        </div>

        <div class="col-lg-4 col-sm-6">

          <h4 id="coordinate">COORDINATE</h4>

          <div class="d-flex">
            <div class="images">
              <img src="../assets/orologio.png" alt="">
            </div>
            <div>
              <h5 class="clr-red">Durata</h5>
              <p>Ottobre - maggio per un totale di 60 ore</p>
            </div>
          </div>

          <div class="d-flex">
            <div class="images">
              <img src="../assets/posizione.png" alt="">
            </div>
            <div>
              <h5 class="clr-red">Sede</h5>
              <p>Il corso si terrà presso la sede di Corus s.a.s. in Via Lautelmonte, 32 a Esine(Brescia)</p>
            </div>
          </div>

          <div class="d-flex">
            <div class="images">
              <img src="../assets/people.png" alt="">
            </div>
            <div>
              <h5 class="clr-red">ORGANIZZAZIONE</h5>
              <p>Gli allievi verranno organizzati in gruppi di massimo 5 persone</p>
            </div>
          </div>

          <div class="d-flex">
            <div class="images">
              <img src="../assets/attestato-icon.png" alt="">
            </div>
            <div>
              <h5 class="clr-red">ATTESTATO DI PARTECIPAZIONE</h5>
            </div>
          </div>

        </div>
      </div>
    </div>

    <!-- striscia rossa  -->
    <div class="bg-red">
      <div class="container">
        <div class="row justify-content-sm-center">
          <div class="col-12 col-md-5 text-center">
            <div>L'allievo può scegliere tra <strong>2 livelli di apprendimento</strong> in base alle conoscenze della lingua già acquisite.</div>
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
.bg-red{
  background-color: red;
  color: white;
  font-size: 20px;
  padding: 20px;
}
.why-cinese{
  margin: 40px 0;
}
#coordinate{
  margin: 20px 0;
}
.images{
  margin-right: 15px;
}
.image{
  position: absolute;
  right: 0;
}

</style>