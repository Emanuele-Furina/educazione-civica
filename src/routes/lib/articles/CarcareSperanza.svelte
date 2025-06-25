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
        <span class="bg-gradient-to-r from-teal-500 to-blue-500 text-white text-sm font-bold px-4 py-2 rounded-full">Società</span>
        <span class="text-gray-500">27 Marzo 2023</span>
        <span class="text-gray-500">9 min di lettura</span>
      </div>
      
      <h1 class="text-4xl md:text-5xl font-bold mb-6 bg-gradient-to-r from-teal-600 to-blue-600 bg-clip-text text-transparent leading-tight">
        Carcere e speranza
      </h1>
      
      <p class="text-xl text-gray-600 leading-relaxed max-w-3xl mx-auto">
        Un viaggio nella realtà del carcere tra teatro, speranza e rieducazione. Esperienze e riflessioni che interrogano la società attraverso lo spettacolo "Le Finestre" e gli incontri con chi lavora dietro le sbarre.
      </p>
    </div>
  </header>
  <div class="prose prose-lg max-w-none space-y-8">
    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-teal-600 to-blue-600 bg-clip-text text-transparent">
        Un carcere, due mondi: dentro e fuori
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Il carcere è spesso raccontato solo come luogo di punizione, ma c'è un altro aspetto, più silenzioso e profondo, che merita attenzione: quello umano, quotidiano, invisibile. In Italia, strutture come il carcere <em>Lorusso e Cotugno</em> di Torino diventano luoghi di esperienze che interrogano la società stessa, non solo chi sta scontando una pena.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Anche se <strong>non ho assistito direttamente allo spettacolo teatrale "Le Finestre"</strong>, presentato il 24 ottobre 2023 all'interno del carcere torinese, il tema e il messaggio che ha veicolato mi hanno profondamente colpito. Lo spettacolo, messo in scena da una compagnia teatrale formata da detenuti e attori esterni, affronta in modo potente la questione della <strong>speranza</strong> in un luogo dove troppo spesso regnano il silenzio e il buio.
      </p>
    </div>

    <div class="bg-gradient-to-r from-amber-50 to-orange-50 rounded-3xl p-8 border-l-4 border-amber-500">
      <h2 class="text-3xl font-bold mb-6 text-amber-800">
        "Le Finestre": un varco tra disperazione e possibilità
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Attraverso il racconto di chi ha visto lo spettacolo, emerge un'immagine chiara: <strong>la speranza è la prima a essere incarcerata</strong>. Spesso, i detenuti vivono il carcere come un tempo sospeso, in cui l'idea del futuro è sfocata. Non manca solo la libertà, ma anche la possibilità di immaginarsi un "dopo".
      </p>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Chi è dentro, anche quando può accedere a benefici o misure alternative, ha spesso paura del mondo esterno. Il rientro nella società può significare emarginazione, disoccupazione, stigma. Lo spettacolo, da quanto mi è stato raccontato, riesce a comunicare tutto questo con intensità, senza pietismo, ma con la forza del teatro: un linguaggio diretto, emotivo, trasformativo.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        La finestra diventa un <strong>simbolo</strong>: uno spiraglio, una soglia tra il carcere e il mondo esterno, tra chi osserva e chi è osservato. Ma anche un ponte tra due realtà che, pur apparentemente opposte, appartengono alla stessa umanità. Nessuno è immune al buio. Forse, è proprio riconoscendoci in quello degli altri che possiamo cominciare a cercare insieme la luce.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
        Il teatro come strumento di cambiamento
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Durante un incontro con <strong>Elisabetta Baro</strong>, membro della compagnia teatrale attiva all'interno del carcere, è emerso chiaramente quanto il <strong>teatro possa rappresentare un potente mezzo di rieducazione</strong>. Non si tratta solo di recitare, ma di imparare a riflettere su sé stessi, di prendere consapevolezza della propria storia e di ciò che si è diventati.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Il teatro in carcere costringe a mettersi a nudo, a lavorare su relazioni, emozioni, parole. In un ambiente dove ogni aspetto della vita è condiviso – persino l'intimità, come il cucinare in cella o la gestione degli spazi personali – l'esperienza teatrale permette una forma di espressione profonda e, per molti, nuova.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-indigo-600 bg-clip-text text-transparent">
        La condizione psichiatrica post-manicomiale
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Il percorso di riflessione sul carcere si è arricchito anche con l'approfondimento sul sistema <strong>manicomiale in Italia</strong> e le sue eredità. Dopo la legge Basaglia, molte strutture sono state chiuse, ma resta aperta la questione dell'inclusione e della dignità delle persone affette da disturbi mentali, soprattutto quelle coinvolte nel sistema penale.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Il carcere, infatti, spesso si sostituisce (impropriamente) a strutture sanitarie che dovrebbero occuparsi di queste fragilità. Il rischio è che la reclusione diventi un contenitore indistinto per tutto ciò che la società non riesce a gestire in altro modo.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-green-600 to-teal-600 bg-clip-text text-transparent">
        Incontro con Cosima Buccoliero – "Senza Sbarre"
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        A concludere il percorso, l'incontro con <strong>Cosima Buccoliero</strong>, autrice del libro <em>Senza Sbarre</em>, ha aggiunto uno sguardo più sistemico alla questione. Il testo propone una riflessione sul <strong>senso della pena</strong> e sull'importanza di non spezzare il legame tra carcere e territorio. In questo, la società ha un ruolo cruciale: <strong>non si può chiedere al detenuto di cambiare se lo si condanna a restare invisibile</strong> anche dopo aver scontato la pena.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Il libro sottolinea come il carcere debba essere un luogo di rieducazione e non solo di punizione, dove il detenuto possa ricostruire la propria identità e prepararsi al reinserimento sociale. Questo richiede un impegno collettivo che va oltre le mura del carcere.
      </p>
    </div>

    <div class="bg-gradient-to-r from-teal-50 to-blue-50 rounded-3xl p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-teal-600 to-blue-600 bg-clip-text text-transparent">
        Conclusione: un invito alla responsabilità collettiva
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Il carcere è uno specchio della società. Ogni volta che ci voltiamo dall'altra parte, contribuendo all'indifferenza e al pregiudizio, dimentichiamo che chi è dentro ha comunque diritto a dignità, educazione, futuro.
      </p>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Anche senza aver partecipato allo spettacolo, ho compreso quanto esperienze come "Le Finestre" non siano semplici attività culturali, ma <strong>atti politici e umani</strong> che ci interrogano. Ci ricordano che aprire una finestra non è solo un gesto fisico, ma un segno di disponibilità: a guardare, a capire, e forse anche ad accogliere.
      </p>
      
      <blockquote class="border-l-4 border-teal-500 pl-6 italic text-lg text-gray-700">
        "Finché esiste una finestra, la prigione è solo una stanza con una possibilità."
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
