<template>
  <div>
      <div class="container">
          <div class="row">
            <div class="col-12">
                <h2 class="clr-red">2 LIVELLI DI APPRENDIMENTO</h2>
                <p>le competenze acquisibili con i corsi di cinese e giapponese in aula</p>
            </div>
        </div>
      </div>
      
    <!-- card di informazione corsi -->
    <div class="container">
        <div class="row">

            <div v-for="corso,i in corsi" :key="i" class="col-sm-6 col-12">
                <img src="" alt="">
                <div class="text-level"><!--devo cambiare l'h dei blocchi in base alla dimensione dello schemro -->
                    <h3 class="clr-red">{{corso.title}}</h3>
                    <p>{{corso.text}}</p>
                </div>
                <div> 
                    <p>{{corso.comment}}</p>
                </div>
            </div>

        </div>
    </div>

    <!-- sezione attestato di partecipazione-->
    <div class="container">
        <div class="row">
            <div class="col-sm-4 col-12">
                <img src="" alt="">
            </div>
            <div class="col-sm-8 col-12">
                al termine di ogni corso, tutti i partecipanti riceveranno un
                <h4 class="clr-red"><strong>ATTESTATO DI PARTECIPAZIONE</strong></h4>
            </div>
        </div>
    </div>

    <div class="bg-lightgray">
        <div class="container">
            <div class="row ">
                <div class="col-sm-4 col-0">
                    <img src="" alt="">
                </div>
                <div class="col-sm-8 col-12">
                    <strong>Contattaci per ricevere tutti i dettagli dei</strong> 
                    <h4 class="clr-red"><strong>CORSI DI LINGUA CINESE E GIAPPONESE IN AULA</strong></h4>
                </div>
            </div>
        </div>
    </div>


  </div>
</template>

<script>
export default {
  name: 'Levels',
  props: {
   corsi:Array,
  }
}
</script>

<style scoped lang="scss">
.text-level{
    height: 300px;
}
.bg-lightgray{
    background-color: rgb(235, 235, 235);
    padding: 20px 0;
}
</style>
