<script>
  let { navigateTo } = $props();
</script>

<article class="max-w-4xl mx-auto">
  <!-- Header dell'articolo -->
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
        <span class="bg-gradient-to-r from-purple-500 to-pink-500 text-white text-sm font-bold px-4 py-2 rounded-full">Letteratura</span>
        <span class="text-gray-500">29 Dicembre 2022</span>
        <span class="text-gray-500">12 min di lettura</span>
      </div>
      
      <h1 class="text-4xl md:text-5xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent leading-tight">
        La pena di morte e l'umanità del condannato
      </h1>
      
      <p class="text-xl text-gray-600 leading-relaxed max-w-3xl mx-auto">
        Un viaggio tra letteratura e realtà, attraverso la riflessione sulla pena di morte e il capolavoro di Victor Hugo, "L'ultimo giorno di un condannato a morte".
      </p>
    </div>
  </header>

  <!-- Contenuto dell'articolo -->
  <div class="prose prose-lg max-w-none">
    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 mb-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
        La giustizia che uccide: riflessioni su un tema universale
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La pena di morte è uno dei temi più controversi e dibattuti della storia dell'umanità. Intesa da alcuni come uno strumento di giustizia estrema, e da altri come una barbarie legalizzata, essa pone interrogativi profondi sull'etica, sul diritto e sulla dignità dell'essere umano. In molti Paesi del mondo è ancora in vigore, mentre in altri è stata abolita o sospesa da decenni. Ma al di là delle legislazioni, resta forte la domanda: è mai giusto togliere la vita a una persona, anche se colpevole?
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        È proprio questo interrogativo che Victor Hugo affronta nel suo intenso romanzo <em>L'ultimo giorno di un condannato a morte</em>, un'opera breve ma potentissima, che non offre risposte facili, ma ci costringe a guardarci dentro.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 mb-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-green-600 to-blue-600 bg-clip-text text-transparent">
        Un romanzo contro la ghigliottina
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Scritto nel 1829, <em>L'ultimo giorno di un condannato a morte</em> è più di un testo letterario: è una denuncia, un atto politico, una meditazione sull'assurdità della pena capitale. Hugo, profondamente contrario alla pena di morte, utilizza la narrativa come strumento di impegno civile, dando voce a chi quella voce l'ha perduta.
      </p>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Il romanzo è un monologo in prima persona. Il protagonista, la cui identità resta volutamente anonima – non ne conosciamo né il nome né il crimine – ci parla dalla sua cella nel carcere di Bicêtre, nei 57 giorni che lo separano dalla ghigliottina. L'autore sceglie di non dirci cosa abbia fatto, perché il centro della narrazione non è il reato, ma l'<strong>uomo</strong>, con le sue paure, i suoi pensieri, le sue speranze.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Sappiamo soltanto che è un marchese, un uomo colto e religioso, che trova conforto nella figura del prete che lo accompagna spiritualmente nell'attesa della morte. Ogni giorno, il condannato si aggrappa alla speranza di una grazia, che però non arriverà mai. E fino all'ultimo minuto, quando il patibolo è ormai inevitabile, resta in lui un filo sottile di illusione, quasi infantile, che qualcosa possa salvarlo.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 mb-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
        L'universalità della sofferenza
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La grande forza dell'opera sta nel suo sguardo umano. Hugo non vuole che ci identifichiamo con il colpevole o con l'innocente, ma con l'uomo in quanto tale. Il condannato non è un mostro, né un martire: è un essere umano che pensa, che ama, che ricorda la figlia piccola che non rivedrà più, che prova terrore per una morte fredda e pubblica, eseguita sotto lo sguardo crudele di una folla assetata di spettacolo.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        La pena di morte, nel romanzo, non viene raccontata tanto come punizione, quanto come <strong>agonia mentale e fisica</strong>. È l'attesa stessa della morte che tortura il protagonista, giorno dopo giorno, togliendogli lentamente ogni briciolo di umanità. E ciò che Hugo vuole mostrare è proprio questo: che nessun crimine può giustificare l'annullamento della dignità umana.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 mb-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-orange-600 to-red-600 bg-clip-text text-transparent">
        Letteratura e impegno civile
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Con quest'opera, Victor Hugo si schiera apertamente contro la pena di morte. E lo fa in un'epoca in cui essa era considerata normale, addirittura necessaria. Ma il romanzo non è mai didascalico: non c'è predica, non c'è giudizio diretto. È la voce del protagonista che, pagina dopo pagina, porta il lettore a interrogarsi, a riflettere, a provare empatia.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Hugo anticipa così una forma moderna di letteratura impegnata, capace di influenzare l'opinione pubblica più della politica. E non è un caso se ancora oggi, a distanza di quasi due secoli, <em>L'ultimo giorno di un condannato a morte</em> viene letto nelle scuole, nelle università, nei circoli dei diritti civili, come manifesto contro ogni forma di giustizia disumana.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 mb-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-red-600 to-pink-600 bg-clip-text text-transparent">
        Pena di morte oggi: una questione ancora aperta
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Sebbene in molti Paesi europei la pena capitale sia stata abolita, essa è ancora oggi applicata in numerose nazioni. Secondo i dati di <strong>Amnesty International</strong>, nel 2023 almeno <strong>1.153 esecuzioni</strong> sono state registrate nel mondo, con punte altissime in Iran, Arabia Saudita e Cina (anche se qui le cifre ufficiali restano segrete). In alcuni casi, la pena di morte viene applicata anche per reati non violenti, come il traffico di droga o i reati politici.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Il dibattito resta acceso. I sostenitori parlano di giustizia, deterrenza e risarcimento morale per le vittime. Gli oppositori denunciano invece l'<strong>irrimediabilità</strong> dell'errore giudiziario, le disuguaglianze sociali che colpiscono soprattutto i poveri e le minoranze etniche, e la disumanità di uno Stato che si arroga il diritto di uccidere.
      </p>
    </div>

    <div class="bg-gradient-to-r from-blue-50 to-purple-50 rounded-3xl p-8 mb-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
        Conclusione: la forza della voce
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        <em>L'ultimo giorno di un condannato a morte</em> ci lascia una lezione semplice e potente: <strong>ogni essere umano ha diritto alla vita e alla dignità</strong>, anche quando ha sbagliato. La giustizia non può trasformarsi in vendetta. E la letteratura, in questo senso, ha un potere immenso: quello di ridare voce a chi l'ha persa, di mostrare ciò che la legge, a volte, ignora.
      </p>

      <!-- Video embed -->
      <div class="bg-white/50 rounded-2xl p-6 mb-6">
        <div class="aspect-video">
          <iframe 
            width="100%" 
            height="100%" 
            src="https://www.youtube.com/embed/EeGa-YNNemk" 
            title="L'ULTIMO GIORNO DI UN CONDANNATO di V. Hugo" 
            frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
            referrerpolicy="strict-origin-when-cross-origin" 
            allowfullscreen
            class="rounded-xl"
          ></iframe>
        </div>
      </div>

      <blockquote class="border-l-4 border-blue-500 pl-6 italic text-lg text-gray-700">
        "L'uomo non ha il diritto di togliere ciò che non ha creato: la vita." – Victor Hugo
      </blockquote>
    </div>
  </div>

  <!-- Navigation footer -->
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
