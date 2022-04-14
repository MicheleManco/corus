<template>
  <div class="bg-gray1">
    <div class="container">
      <div class="row">

        <div class="col-4 d-none d-xl-flex justify-content-end ">
          <div class="bg-gray2 robotoB">Richiedi <br> Informazioni</div>
        </div>

        <!-- form ------------------------------------------------------------------------------------------------------------------ -->
        <form action="" class="row col-xl-8 needs-validation spaziatura-col-2" novalidate>
          <div class="col-xl-4 col-md-4 spaziatura-col-2">
            <label for="validationCustom01" class="form-label padding-blocco">Nome e Cognome *</label>
            <input type="text" class="no_border_radius form-control formH margin-blocco" id="validationCustom01" value="" required>

            <label class="spazioform form-label padding-blocco">Telefono</label>
            <input class="inputs no_border_radius form-control formH margin-blocco" type="tel">

            <label for="exampleInputEmail1" class="spazioform form-label">E-mail *</label>
          <input class="inputs no_border_radius form-control formH margin-blocco" id="exampleInputEmail1" required type="email">

            <div class="spazioform">Corso di interesse</div>
            <select class="no_border_radius inputs selection formH" name="interesse">
              <option value="Cinese-Base">Cinese Base</option>
              <option value="Cinese-Elementare">Cinese Elementare</option>
              <option value="Giapponese-Base">Giapponese Base</option>
              <option value="Giapponese-Elementare">Giapponese Elementare</option>
            </select>
          </div>

          <div class="col-xl-6 col-md-8">
            <label class="form-label" for="validationTextarea">Messaggio *</label>
            <textarea class="no_border_radius form-control" id="validationTextarea"  name=""  required></textarea>

            <div class="d-xxl-flex justify-content-between check-container align-items-center">
              <div class="d-flex flex-nowrap">
                <input class="checkbox form-check-input" type="checkbox" value="" id="invalidCheck" required name="termini">
                <a href=""><label class="form-check-label fs7" for="invalidCheck">Accettazione Tratt. Dati Personali *</label></a>
              </div>
              <div class="fs7">* campi obbligatori</div>
            </div>

            <div class="d-flex justify-content-end btn-invio">
              <button class="invia_richiesta" type="submit"><div>Invia Richiesta<img src="../assets/arrow-right.png" alt=""></div></button> 
            </div>
          </div>
        </form>
        <!-- end-form ---------------------------------------------------------------------------------------------------- -->

        <div class="info-corus">
          <div class="col-12 text-center fs-6 robotoB">Corus s.a.s. - Servizi di traduzione ed interpretariato in Cinese, Giapponese e Coreano</div>
          <div class="col-12 text-center fs-6">Via Leutelmonte 32, 25040 ESINE (BS) - P.IVA:02251300980 | privacy cookies policy</div>
        </div>
        
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'Footer',
  methods:{
    validazione () {

    // Fetch all the forms we want to apply custom Bootstrap validation styles to
    var forms = document.querySelectorAll('.needs-validation')

    // Loop over them and prevent submission
      Array.prototype.slice.call(forms)
      .forEach(function (form) {
        form.addEventListener('submit', function (event) {
          if (!form.checkValidity()) {
            event.preventDefault()
            event.stopPropagation()
          }

          form.classList.add('was-validated')
        }, false)
      })
    }
  },
  mounted(){
   this.validazione()
  }
}
</script>

<style scoped lang="scss">
.fs7{
font-size: 13px;
}
.form-check-input{
  border-radius: 0;
}
.robotoB{
   font-family: 'Roboto';
   font-weight: 700;
}
.fs-6{
  line-height: 21px;
}
.formH{
  height: 32px;
}
label{
  margin-bottom: 0px;
}
.check-container{
  margin-top: 15px;
}
.no_border_radius{
  border-radius: 0px;
}
a{
  color: white;
  .form-check-label{
    text-decoration: underline;
    margin-left: 10px;
  }
}
.bg-gray1{
  background-color: #4c4c4c;
  color: white;
  padding-top: 30px;
  .bg-gray2{
    background-color: #313131;
    font-size: 30px;
    line-height: 35px;
    height: 145px;
    width: 260px;
    padding: 37px 27px;
    margin-top: -50px;
  }
}
.spaziatura-col-2{
  padding:0 20px 0 16px;
}
.inputs{
  width: 100%;
  border-radius: 0;
}
.inputs:focus {
  
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
  background-color: #ff9f19;
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