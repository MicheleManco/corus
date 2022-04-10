<template>
  <div id="app">
    <Jumbotron/>
    <WhyC/>
    <WhyJ/>
    <Info/>
    <Levels :corsi = "corsi"/>
    <Footer/>
  </div>
</template>

<script>
import Jumbotron from './components/Jumbotron.vue'
import WhyC from './components/WhyC.vue'
import WhyJ from './components/WhyJ.vue'
import Info from './components/Info.vue'
import Levels from './components/Levels.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Jumbotron,
    WhyC,
    WhyJ,
    Info,
    Levels,
    Footer
  },
  data(){
    return {
      corsi: [
        // corso1
        {
          title: "CORSO BASE DI CINESE (A1)",
          text:"il corso base è rivolto a chi è interessato a un primo approccio alla lingua cinese e vuole approfondire aspetti peculiari della cultura locale.Nel corso delle lezioni gli studenti impareranno la fonetica, il pinyin, le nozionibase della scrittura e le principali scritture grammaticali; saranno così  in grado di formulare frasi semplici, ma utili nella vita quotidiana e per presentare se stessi agli altri.",
          comment:"Al termine del corso si prevede il raggiungimento del livello A1 del Quadro comune europeo di riferimento per le lingue",
          image:"assets/primo-pallino.png"
        },
        //corso2
        {
          title:"CORSO BASE DI GIAPPONESE (A1)",
          text:"Il corso base è rivolto a chi è interessato a un primo approccio alla lingua giapponese, abbinato a uno sguardo alle tradizioni e peculiarità del Paese del 'Sol Levante'. Nel corso delle lezioni gli studenti impareranno a leggere e scrivere in hiragana e katakana, venendo introdotti in seguito all'utilizzo dei kanji. A ciò si aggiungerà l'insegnamento delle regole grammaticali di base, con esercizi e dialoghi riguardanti gli ambiti più comuni, che permetteranno ai partecipanti di poter interagire in modo semplice, utilizzare espressioni quotidiane e presentare sé stessi e gli altri",
          comment:"Al termine del corso si prevede il raggiungimento del livello A1 del Quadro comune europeo di riferimento per le lingue.",
          image:"assets/primo-pallino.png"
        },
        {
          title:"CORSO ELEMENTARE DI CINESE (A2)",
          text:"Il corso elementare è indirizzato a tutti coloro che, avendo una conoscenza basilare della lingua cinese, vogliono continuare il loro percorso di apprendimento. Durante le lezioni i partecipanti acquisiranno maggiore dimestichezza con la lingua viva riuscendo a esprimersi in modo chiaro in molteplici situazioni quotidiane. Per questo livello è prevista l'interazione di due docenti, docente madrelingua per la fonetica e conversazione.",
          comment:"Al termine del corso si prevede il raggiungimento del livello A2 del Quadro comune europeo di riferimento per le lingue. Se interessati gli studenti potranno iscriversi con il nostro supporto all'esame HSK2",
          image:"assets/secondo-pallino.png"
        },
        {
          title:"CORSO ELEMENTARE DI GIAPPONESE (A2)",
          text:"Il corso elementare di lingua giapponese è indirizzato a tutti coloro che, avendo una conoscenza basilare della lingua giapponese, vogliono continuare il loro percorso di apprendimento. Nel corso delle lezioni gli studenti impareranno nuovi kanji, strutture grammaticali ed espressioni di uso comune che permetteranno loro di potersi esprimere, in termini semplici, riguardo contesti familiari, aspetti della propria vita e dell'ambiente circostante. Sapranno quindi chiedere e dare indicazioni, descrivere ciò che accade attorno a sé e interagire in situazioni abituali con maggior scioltezza. Parimenti al corso base, alcuni momenti verranno dedicati all'approfondimento di temi riguardanti la società e la cultura giapponese.",
          comment:"Al termine del corso si prevede il raggiungimento del livello A2 del Quadro comune europeo di riferimento per le lingue.",
          image:"assets/secondo-pallino.png"
        }

      ],
    }
  },
}
</script>

<style lang="scss">

.clr-red{
  color: red;
}
</style>
