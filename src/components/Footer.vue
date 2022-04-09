<template>
  <div class="bg-gray1">
    <div class="container">
      <div class="row">

        <div class="col-4">
          <div class="bg-gray2">Richiedi Informazioni</div>
        </div>

        <div class="col-2">
          <div>Nome e Cognome*</div>
          <input type="text">
          <div>telefono</div>
          <input type="text">
          <div>E-mail*</div>
          <input type="text">
          <div>Corso di interesse</div>
          <select name="interesse">
            <option value="Cinese-Base"> Cinese Base</option>
            <option value="Cinese-Elementare"> Cinese Elementare</option>
            <option value="Giapponese-Base"> Giapponese Base</option>
            <option value="Giapponese-Elementare"> Giapponese Elementare</option>
          </select>
        </div>

        <div class="col-6">
          <div>Messaggio*</div>
          <div><textarea name=""></textarea></div>

          <div>
            <input type="checkbox" name="termini"><a href=""> Accettazione Tratt. Dati Personali</a>
            <div>*campi obbligatori</div>
          </div>

          <div>Invia Richiesta <img src="../assets/arrow-right.png" alt=""></div> 
        </div>

        <div class="col-12 text-center"><strong>Corus s.a.s. - Servizi di traduzione ed interpretariato in Cinese, Giapponese e Coreano</strong></div>
        <div class="col-12 text-center">Via Leutelmonte 32, 25040 ESINE (BS) - P.IVA:02251300980 | privacy cookies policy</div>
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
.bg-gray1{
  background-color: gray;
  .bg-gray2{
    background-color: rgb(65, 65, 65);
  }
}
</style>