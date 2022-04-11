<template>
  <div class="bg-gray1">
    <div class="container">
      <div class="row">

        <div class="col-3 d-none d-xl-block">
          <div class="bg-gray2">Richiedi <br> Informazioni</div>
        </div>

        <!-- form ------------------------------------------------------------------------------------------------------------------ -->
        <form action="" class="row col-xl-9  spaziatura-col-2">
          <div class="col-xl-3 col-md-4 spaziatura-col-2">
            <div>Nome e Cognome *</div>
            <input class="inputs" type="text">

            <div class="spazioform">telefono</div>
            <input class="inputs" type="text">

            <div class="spazioform">E-mail *</div>
            <input class="inputs" type="text">

            <div class="spazioform">Corso di interesse</div>
            <select class="inputs selection" name="interesse">
              <option value="Cinese-Base">Cinese Base</option>
              <option value="Cinese-Elementare">Cinese Elementare</option>
              <option value="Giapponese-Base">Giapponese Base</option>
              <option value="Giapponese-Elementare">Giapponese Elementare</option>
            </select>
          </div>

          <div class="col-xl-6 col-md-8">
            <div>Messaggio *</div>
            <textarea name=""></textarea>

            <div class="d-xxl-flex justify-content-between">
              <div><input type="checkbox" name="termini"><a class="accettazione" href=""> Accettazione Tratt. Dati Personali</a> *</div>
              <div>* campi obbligatori</div>
            </div>

            <div class="d-flex justify-content-end btn-invio">
              <button class="invia_richiesta" type="submit"><div>Invia Richiesta<img src="../assets/arrow-right.png" alt=""></div></button> 
            </div>
          </div>
        </form>
        <!-- end-form ---------------------------------------------------------------------------------------------------- -->

        <div class="info-corus">
          <div class="col-12 text-center"><strong>Corus s.a.s. - Servizi di traduzione ed interpretariato in Cinese, Giapponese e Coreano</strong></div>
          <div class="col-12 text-center">Via Leutelmonte 32, 25040 ESINE (BS) - P.IVA:02251300980 | privacy cookies policy</div>
        </div>
        
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'Footer',
  props: {
   
  }
}
</script>

<style scoped lang="scss">
a{
  color: white;
}
.bg-gray1{
  background-color: rgb(65, 65, 65);
  color: white;
  padding-top: 30px;
  .bg-gray2{
    background-color: rgb(32, 32, 32);
    font-size: 30px;
    line-height: 35px;
    height: 145px;
    width: 248px;
    padding: 37px 27px;
    margin-top: -50px;
  }
}
.spaziatura-col-2{
  padding-right: 20px;
}
.inputs{
  width: 100%;
}
.spazioform{
  margin-top: 10px;
}
textarea{
  resize: none;
  width: 100%;
  height: 85px;
}
.btn-invio{
  margin-top: 18px;
}
.invia_richiesta{
  color: black;
  height: 55px;
  width: 240px;
  font-size: 19px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #dc8122;
  border:none;
  img{
    margin-left: 25px;
  }
}
.info-corus{
  margin: 55px 0;
}

.selection{
  margin-bottom: 10px;
}

</style>