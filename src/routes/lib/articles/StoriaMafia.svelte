<script>
  let { navigateTo } = $props();
</script>

<article class="max-w-4xl mx-auto">
  <header class="mb-12">
    <button 
      onclick={() => navigateTo('blog')}
      class="flex items-center text-blue-600 hover:text-blue-800 mb-6 font-medium transition-colors duration-300"
    >
      <svg class="w-5 h-5 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"></path>
      </svg>
      Torna al Blog
    </button>

    <div class="text-center">
      <div class="flex items-center justify-center space-x-4 mb-6">
        <span class="bg-gradient-to-r from-red-500 to-orange-500 text-white text-sm font-bold px-4 py-2 rounded-full">Storia</span>
        <span class="text-gray-500">22 Marzo 2022</span>
        <span class="text-gray-500">15 min di lettura</span>
      </div>
      
      <h1 class="text-4xl md:text-5xl font-bold mb-6 bg-gradient-to-r from-red-600 to-orange-600 bg-clip-text text-transparent leading-tight">
        La Storia della Mafia e le Stragi
      </h1>
      
      <p class="text-xl text-gray-600 leading-relaxed max-w-3xl mx-auto">
        Un approfondito viaggio attraverso la storia della mafia italiana, dalle origini ottocentesche alle stragi degli anni '90, per comprendere e non dimenticare chi ha sacrificato la vita per la legalità.
      </p>
    </div>
  </header>

  <div class="prose prose-lg max-w-none space-y-8">
    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-red-600 to-orange-600 bg-clip-text text-transparent">
        Le Origini della Mafia in Sicilia
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La mafia siciliana nasce nell'Ottocento come fenomeno legato al controllo delle terre e dei rapporti sociali nell'isola. Dopo l'Unità d'Italia, in un contesto di debolezza dello Stato centrale, emergono gruppi criminali che si sostituiscono alle autorità nel controllo del territorio. La mafia non è solo criminalità comune, ma un sistema di potere che mescola violenza, codici d'onore e connivenze con il potere politico ed economico.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Le prime manifestazioni del fenomeno mafioso si concentrano nelle campagne palermitane, dove i "gabellotti" (amministratori delle terre) assumono uomini armati per proteggere le proprietà. Questi gruppi paramilitari evolveranno gradualmente in vere e proprie cosche mafiose, caratterizzate da rigide gerarchie interne e dal controllo violento del territorio.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-orange-600 to-yellow-600 bg-clip-text text-transparent">
        L'Evoluzione nel Novecento
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Durante il fascismo, il prefetto Cesare Mori condusse una durissima repressione contro la mafia siciliana, ottenendo risultati significativi ma temporanei. La caduta del regime e lo sbarco degli Alleati in Sicilia nel 1943 segnarono la rinascita del potere mafioso, spesso con la complicità delle forze di occupazione che vedevano nei mafiosi degli alleati contro il comunismo.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Nel secondo dopoguerra, la mafia si modernizza e si espande, entrando nel traffico di stupefacenti e stabilendo collegamenti internazionali. La "Cosa Nostra" siciliana diventa una delle organizzazioni criminali più potenti al mondo, estendendo la sua influenza negli Stati Uniti attraverso l'emigrazione siciliana.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
        Il Maxiprocesso e la Reazione Mafiosa
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Gli anni '80 rappresentano una svolta nella lotta alla mafia. I magistrati Giovanni Falcone e Paolo Borsellino, supportati dal lavoro investigativo del generale Carlo Alberto Dalla Chiesa (assassinato nel 1982), costruiscono un imponente apparato accusatorio basato sulle rivelazioni di Tommaso Buscetta, primo pentito di rilievo di Cosa Nostra.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Il Maxiprocesso, iniziato nel 1986 nell'aula bunker del carcere dell'Ucciardone a Palermo, porta alla condanna di centinaia di mafiosi. Il processo dimostra per la prima volta l'esistenza di Cosa Nostra come organizzazione unitaria e gerarchicamente strutturata, smontando la tesi dei "semplici" delinquenti comuni.
      </p>
    </div>

    <div class="bg-gradient-to-r from-red-50 to-orange-50 rounded-3xl p-8 border-l-4 border-red-500">
      <h2 class="text-3xl font-bold mb-6 text-red-800">
        Le Stragi del 1992-1993
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La reazione di Cosa Nostra alle condanne definitive del Maxiprocesso è feroce e senza precedenti. Il <strong>23 maggio 1992</strong>, sull'autostrada A29 presso Capaci, un attentato dinamitardo uccide il giudice <strong>Giovanni Falcone</strong>, la moglie Francesca Morvillo e gli agenti della scorta Antonio Montinaro, Rocco Dicillo e Vito Schifani.
      </p>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Due mesi dopo, il <strong>19 luglio 1992</strong>, in via D'Amelio a Palermo, un'autobomba esplosiva uccide <strong>Paolo Borsellino</strong> e cinque agenti della sua scorta: Emanuela Loi, Agostino Catalano, Claudio Traina, Eddie Walter Cosina e Vincenzo Li Muli. Emanuela Loi è la prima donna poliziotto a morire per mano della mafia.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Le stragi continuano nel 1993 spostandosi in continente: Roma, Firenze e Milano vengono colpite da attentati dinamitardi che causano morti e feriti, oltre a danni inestimabili al patrimonio artistico (Uffizi, San Giorgio al Velabro, San Giovanni in Laterano).
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-green-600 to-blue-600 bg-clip-text text-transparent">
        Peppino Impastato: Una Voce Contro il Silenzio
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Giuseppe Impastato rappresenta una delle figure più significative della resistenza civile alla mafia. Nato a Cinisi nel 1948, Peppino cresce in un ambiente dove la presenza mafiosa è pervasiva e spesso tollerata. Suo padre Luigi ha legami con Cosa Nostra, ma Peppino sceglie la strada opposta, diventando un attivista politico e giornalista.
      </p>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La sua battaglia inizia negli anni '70 attraverso Radio Aut, l'emittente che fonda per denunciare i traffici illeciti e la presenza mafiosa nel territorio. Le sue trasmissioni, caratterizzate da ironia tagliente e coraggio, prendono di mira direttamente Gaetano Badalamenti, potente boss di Cinisi coinvolto nel traffico internazionale di eroina.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Il <strong>9 maggio 1978</strong>, a soli trent'anni, Peppino viene assassinato con una carica di tritolo. Il suo corpo viene fatto saltare sui binari della ferrovia per simulare un incidente o un suicidio. Solo anni dopo, grazie alle battaglie della madre Felicia Bartolotta e del Centro Siciliano di Documentazione "Giuseppe Impastato", la verità emerge: Peppino è stato ucciso dalla mafia per le sue denunce.
      </p>

      <div class="bg-white/50 rounded-2xl p-6 mt-6">
        <div class="aspect-video">
          <iframe 
            width="100%" 
            height="100%" 
            src="https://www.youtube.com/embed/ag1_vfwzgFA" 
            title="Peppino Impastato" 
            frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
            allowfullscreen
            class="rounded-xl"
          ></iframe>
        </div>
      </div>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
        L'Eredità di Falcone e Borsellino
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Giovanni Falcone e Paolo Borsellino hanno rivoluzionato l'approccio investigativo alla criminalità organizzata, introducendo metodi innovativi che sono diventati standard internazionali. Il loro lavoro ha dimostrato che la mafia può essere sconfitta attraverso la determinazione, la competenza e il coraggio.
      </p>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Falcone sviluppa il metodo di indagine patrimoniale, seguendo i flussi di denaro per ricostruire le attività criminali. Introduce l'uso sistematico delle intercettazioni telefoniche e ambientali, crea una banca dati informatica per analizzare i collegamenti tra i diversi clan mafiosi.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Entrambi comprendono l'importanza della comunicazione con l'opinione pubblica: partecipano a convegni, rilasciano interviste, scrivono articoli per spiegare il loro lavoro e sensibilizzare la società civile sulla gravità del fenomeno mafioso.
      </p>
    </div>

    <div class="bg-gradient-to-r from-blue-50 to-purple-50 rounded-3xl p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
        Educazione alla Legalità
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La battaglia contro la mafia non può essere vinta solo con gli strumenti repressivi: è fondamentale un lavoro culturale e educativo che coinvolga le nuove generazioni. Le scuole italiane hanno introdotto percorsi di educazione alla legalità che utilizzano le storie di Falcone, Borsellino, Impastato come esempi di coraggio civile.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        La memoria delle vittime diventa strumento di riscatto: attraverso il ricordo di chi ha sacrificato la vita per la giustizia, si costruisce una coscienza collettiva capace di opporsi alla cultura mafiosa.
      </p>
      
      <blockquote class="border-l-4 border-blue-500 pl-6 italic text-lg text-gray-700 mt-8">
        "La memoria è l'arma più potente contro l'oblio e l'indifferenza. Non dimentichiamo."
      </blockquote>
    </div>
  </div>

  <footer class="mt-16 pt-8 border-t border-gray-200">
    <div class="flex justify-between items-center">
      <button 
        onclick={() => navigateTo('blog')}
        class="flex items-center text-blue-600 hover:text-blue-800 font-medium transition-colors duration-300"
      >
        <svg class="w-5 h-5 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"></path>
        </svg>
        Torna al Blog
      </button>
      
      <div class="flex space-x-4">
        <button class="bg-blue-100 text-blue-800 px-4 py-2 rounded-lg hover:bg-blue-200 transition-colors duration-300">
          Condividi
        </button>
        <button class="bg-gray-100 text-gray-800 px-4 py-2 rounded-lg hover:bg-gray-200 transition-colors duration-300">
          Stampa
        </button>
      </div>
    </div>
  </footer>
</article>
