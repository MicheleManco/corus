<template>
  <div class="big-container">
    <div class="container">
      <div class="row core d-flex justify-content-center">

        <div class="col-lg-9 col-12 row d-flex ">

          <div class="col-2 d-none d-xl-block"> <!--spaziatore --></div>

          <div class="row col-12 col-lg-10 container-middle">
            <div class="col-12 d-none d-xl-block spazio-titolo-top"></div>
            <div class="col-12">
              <div class="main-title robotoB">Corsi di Lingua</div>
              <div class="main-title robotoB">Cinese e Giapponese</div>
            </div>
            <div class="col-12 row">
              <div class="col-3 d-none d-xl-block"></div>
              <div class="col-lg-9 col-12">
                <div class="titolo-lista">corsi in aula a Brescia</div>

                <div class="clr-white d-flex">
                  <img src="../assets/check-yellow.png" alt="">
                  <div class="lista robotoB row-margin-bottom">2 livelli di apprendimento (A1 e A2)</div>
                </div>

                <div class="clr-white d-flex">
                  <img src="../assets/check-yellow.png" alt="">
                  <div class="lista robotoB row-margin-bottom">docenti qualificati</div>
                </div>

                <div class="clr-white d-flex">
                  <img src="../assets/check-yellow.png" alt="">
                  <div class="lista"> <span class=" robotoB"> attestato di partecipazione</span> rilasciato al termine del corso</div>
                </div>
    
              </div>
            </div>
          </div>

          <div class="col-12 d-none d-lg-flex bg-gray align-self-end justify-content-between align-items-center">
            <div>
              <div class="titoletto-giallo robotoB">PARTECIPA AI CORSI IN AULA</div>
              <div class="sottotitolo-bianco robotoB fs-4">e apprendi la lingua cinese e giapponede da docenti qualificati</div>
              <div class="white-text">termine iscrizioni 7 Ottobre</div>
            </div>
            <img id="arrow-white" src="../assets/arrow-wh-right.png" alt="">
          </div>

        </div>

        <!-- form------------------------------------------------------------------------------------------------------------------------------------------------------------->
        <form class="col-3 bg-light-black position-relative needs-validation" id="form-container" novalidate action="">
        <div>
          
          <div class="colore-orange head-form d-flex align-items-center"><div class="da_ottobre">da ottobre 2018</div></div>

          <div class="padding-blocco richiedi_info robotoB">Richiedi informazioni</div>

          <label for="validationCustom01" class="form-label padding-blocco">Nome e Cognome *</label>
          <input type="text" class="no_border_radius form-control margin-blocco formH" id="validationCustom01" value="" required>

          <div class="padding-blocco">telefono</div>
          <input class="margin-blocco formH" type="tel">

          <label for="exampleInputEmail1" class="padding-blocco form-label">E-mail *</label>
          <input class="no_border_radius margin-blocco form-control formH" id="exampleInputEmail1" required type="email">

          <div class="padding-blocco">Corso di interesse</div>
          <select class="no_border_radius margin-blocco formH" name="interesse">
            <option value="Cinese-Base" selected > Cinese Base</option>
            <option value="Cinese-Elementare"> Cinese Elementare</option>
            <option value="Giapponese-Base"> Giapponese Base</option>
            <option value="Giapponese-Elementare"> Giapponese Elementare</option>
          </select>

          <label class="padding-blocco form-label" for="validationTextarea">Messaggio *</label>
          <textarea class="no_border_radius margin-blocco form-control" id="validationTextarea"  name=""  required></textarea>

          <div>
            <div class="padding-blocco">* campi obbligatori</div>
            <div class="checkbox-container">
              <input class="checkbox form-check-input" type="checkbox" value="" id="invalidCheck" required name="termini"> <a href="">
                <label class="form-check-label" for="invalidCheck">Accettazione Tratt. Dati Personali*</label>
              </a> 
            </div>
          </div>

          <button class="invia_richiesta" type="submit"><div>Invia Richiesta<img src="../assets/arrow-right.png" alt=""></div></button>

        </div>
        </form>
        <!-- end form ------------------------------------------------------------------------------------------------------------------------------------------------------------------->
      </div>
    </div>
  </div>
  
</template>

<script>
export default {
  name: 'jumbotron',
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
.robotoB{
   font-family: 'Roboto';
   font-weight: 700;
}
label{
  margin-bottom: 0px;
}
.lista{
  font-size: 22px;
  line-height: 23px;
}
.row-margin-bottom{
  margin-bottom: 50px;
}
.form-check-label{
  margin-left: 5px;
}
#form-container{
  min-height: 670px;
  padding-bottom: 87px;
}
.form-check-label{
    text-decoration: underline;
  }
.no_border_radius{
  border-radius: 0px;
}
.big-container{
  background-image: url("../assets/jumbotron.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: top;
  padding-top: 80px;
}
.spazio-titolo-top{
  height: 110px;
}
.main-title{
  color: white;
  font-size: 60px;
  line-height: 60px;
  margin-left: 124px;
  margin-right: -10px;
}
.titolo-lista{
  color: white;
  font-size: 27px;
  margin: 50px 0px 20px 142px;
}
.clr-white{
  color: white;
  margin-left: 150px;
  img{
    margin-right: 10px;
    width: 26px;
    height: 24px;
  }
}

.colore-orange {
  background-color: #ff9f19;
}
.head-form{
  color: white;
  width: 100%;
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
textarea{
  resize: none;
}
.formH{
  height: 32px;
}
.margin-blocco{
  margin: 0 20px;
  width: 230px;
}
.richiedi_info{
  font-size: 30px;
  line-height: 30px;
  margin: 15px 0;
}

.invia_richiesta{
  height: 85px;
  width:100%;
  font-size: 19px;
  color: rgb(39, 39, 39);
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #ff9f19;
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
  width: 270px;
  padding: 0;
}
.checkbox-container{
  margin: 10px 0;
  display: flex;
  flex-wrap: nowrap;
  align-items: center;
}
a{
  font-size: 13px;
  color: white;
  line-height: 14px;
}
.bg-gray{
  margin-top: 40px;
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
@media all and (max-width: 1200px){
  .main-title{
    margin-left: 0px;
  }
  .clr-white{
  margin-left: 0px;
  }
  .bg-light-black{
  width: 250px;
  padding: 0;
  }
  .margin-blocco{
    margin: 0 20px;
    width: 210px;
  }
  .titolo-lista{
    margin-left: 0px;
  }
}

@media all and (max-width: 991px) {
.big-container{
  padding-top: 15px;
  padding-bottom: 20px;
}

 .bg-light-black{
  width: 80%;
  padding: 0;
  }
  .margin-blocco{
    margin: 0 20px;
    width: 90%;
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
@media all and (max-width: 467px){
.bg-light-black{
  width: 220px;
  padding: 0;
  }
  .margin-blocco{
    margin: 0 20px;
    width: 180px;
  }
}

</style>
