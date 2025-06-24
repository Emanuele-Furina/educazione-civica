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
        <span class="bg-gradient-to-r from-pink-500 to-purple-500 text-white text-sm font-bold px-4 py-2 rounded-full">Società</span>
        <span class="text-gray-500">30 Novembre 2022</span>
        <span class="text-gray-500">10 min di lettura</span>
      </div>
      
      <h1 class="text-4xl md:text-5xl font-bold mb-6 bg-gradient-to-r from-pink-600 to-purple-600 bg-clip-text text-transparent leading-tight">
        La violenza di genere e i femminicidi
      </h1>
      
      <p class="text-xl text-gray-600 leading-relaxed max-w-3xl mx-auto">
        Un'analisi del fenomeno della violenza di genere tra storia, società e dati, per comprendere meglio una delle più gravi emergenze sociali del nostro tempo.
      </p>
    </div>
  </header>

  <!-- Contenuto dell'articolo -->
  <div class="prose prose-lg max-w-none space-y-8">
    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-pink-600 to-purple-600 bg-clip-text text-transparent">
        Un fenomeno antico, una lotta sempre attuale
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La violenza sulle donne non è una realtà nata nel nostro tempo, ma affonda le sue radici in una lunga storia di disuguaglianze. Già nell'antica Roma, la vicenda di Lucrezia – simbolo della donna vittima della brutalità maschile – rappresentava un tragico esempio di sopruso e sopraffazione. Da allora, la strada verso la consapevolezza e la tutela delle vittime è stata lunga e spesso segnata da indifferenza, silenzi e ostacoli.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Oggi, seppur molto è cambiato grazie a battaglie culturali, leggi e mobilitazioni, la violenza di genere resta un'emergenza grave e diffusa. L'introduzione del <strong>Codice Rosso</strong> nel 2019 ha rappresentato un passo importante nella lotta alla violenza domestica e allo stalking, velocizzando le procedure di intervento e rafforzando la protezione per le vittime. Tuttavia, la cronaca continua a riportare casi di donne uccise da chi dichiarava di amarle, segno che la strada verso un reale cambiamento culturale è ancora lunga.
      </p>
    </div>

    <div class="bg-gradient-to-r from-orange-50 to-red-50 rounded-3xl p-8 border-l-4 border-orange-500">
      <h2 class="text-3xl font-bold mb-6 text-orange-800">
        Il significato del 25 novembre
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Ogni anno, il 25 novembre si celebra la <strong>Giornata internazionale per l'eliminazione della violenza contro le donne</strong>, istituita nel 1999 dalle Nazioni Unite. La scelta di questa data non è casuale: ricorda il brutale assassinio delle sorelle Mirabal, tre attiviste politiche della Repubblica Dominicana uccise nel 1960 per il loro impegno contro la dittatura.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        In Italia, questa giornata è occasione per dare voce a chi spesso non ne ha. Nel 2023, la Biblioteca Universitaria di Torino ha organizzato l'evento <em>"Da Lucrezia al Codice Rosso"</em>, durante il quale è stato presentato un archivio digitale che raccoglie documenti, fotografie e testimonianze del movimento femminile italiano. Un patrimonio prezioso, ora accessibile grazie al sito dell'UDI (Unione Donne in Italia), che racconta decenni di lotte, conquiste e resistenza.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-red-600 to-pink-600 bg-clip-text text-transparent">
        Una realtà fatta di numeri, ma anche di silenzi
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La violenza sulle donne non è solo una questione culturale, ma anche una realtà concreta fatta di dati drammatici. Secondo l'<strong>ISTAT</strong>, il 31,5% delle donne italiane tra i 16 e i 70 anni ha subito nel corso della vita violenza fisica o sessuale. Di queste, una su cinque ha subito gravi forme di abuso da parte di partner o ex partner.
      </p>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Nel solo <strong>2023</strong>, 69 donne sono state uccise in Italia. Di queste, ben 64 sono state vittime di partner o ex, a conferma di un modello purtroppo ricorrente: la violenza più pericolosa si consuma spesso tra le mura di casa, in un contesto di apparente intimità.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Durante la pandemia da COVID-19, la situazione è peggiorata drasticamente. Il numero di chiamate al numero antiviolenza <strong>1522</strong> è aumentato del 60% rispetto agli anni precedenti. Le restrizioni e il lockdown hanno costretto molte donne a vivere isolate, in convivenza forzata con il proprio aggressore, privandole del sostegno di amici, familiari o centri di assistenza.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-purple-600 to-blue-600 bg-clip-text text-transparent">
        Quando le leggi non bastano
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Nonostante le normative esistenti, le misure di protezione spesso si rivelano insufficienti. Molte vittime di femminicidio avevano già denunciato violenze, minacce o stalking, ma non sono state protette adeguatamente. Il sistema giudiziario, rallentato e sovraccarico, non sempre riesce a intervenire in tempo. I dispositivi come il braccialetto elettronico, utili per monitorare i movimenti degli aggressori, non sono ancora applicati in modo sistematico.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        A peggiorare il quadro contribuisce la <strong>carenza cronica di fondi</strong>. I <strong>centri antiviolenza</strong> e le <strong>case rifugio</strong>, che rappresentano l'ultima ancora di salvezza per molte donne, operano spesso con risorse limitate e personale ridotto. Questo porta a lunghe liste d'attesa, impossibilità di accogliere tutte le richieste e servizi psicologici o legali non sempre garantiti.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-green-600 bg-clip-text text-transparent">
        Radici culturali e nuove forme di violenza
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La violenza sulle donne non si esaurisce nei numeri dei femminicidi. Esiste anche una <strong>violenza più sottile</strong>, ma altrettanto distruttiva: quella simbolica. Si manifesta attraverso stereotipi, linguaggio sessista, rappresentazioni mediatiche distorte, pressioni sull'aspetto fisico e ruoli imposti. In questa logica, il corpo della donna diventa spesso oggetto di controllo e giudizio.
      </p>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Le strutture patriarcali che storicamente hanno definito le relazioni di potere tra i sessi sono ancora vive e influenzano leggi, abitudini e mentalità. Il linguaggio stesso – se non attento – può perpetuare discriminazioni. Per questo è importante usare parole inclusive, evitare espressioni sessiste e promuovere una comunicazione rispettosa.
      </p>
      
      <p class="text-gray-700 leading-relaxed">
        Nell'era digitale, poi, si sono affacciate <strong>nuove forme di violenza</strong>, meno visibili ma molto invasive. Il <strong>cyberstalking</strong>, la <strong>revenge porn</strong>, le molestie via social network e il controllo digitale (ad esempio tramite app di tracciamento) sono strumenti che molti aggressori utilizzano per esercitare potere sulle vittime anche a distanza. Le leggi stanno cercando di adeguarsi, ma spesso manca ancora una piena comprensione del fenomeno da parte di chi dovrebbe garantire la tutela.
      </p>
    </div>

    <div class="bg-gradient-to-r from-green-50 to-blue-50 rounded-3xl p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-green-600 to-blue-600 bg-clip-text text-transparent">
        Prevenzione, educazione, memoria
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Affrontare la violenza di genere significa soprattutto <strong>prevenire</strong>. Serve un'educazione affettiva, al rispetto e alla parità di genere sin dalle scuole primarie. È importante formare insegnanti, medici, operatori sociali, forze dell'ordine, affinché sappiano riconoscere i segnali di abuso e intervenire con competenza.
      </p>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        La <strong>memoria</strong> ha un ruolo centrale. Ricordare le vittime di femminicidio, conoscere i loro nomi e le loro storie, non è solo un atto di rispetto, ma anche un modo per mantenere viva la coscienza collettiva. Gli archivi digitali, come quelli dell'UDI, servono a farci capire quanto è stato fatto, ma anche quanto resta ancora da fare.
      </p>

      <!-- Video embed -->
      <div class="bg-white/50 rounded-2xl p-6 mb-6">
        <div class="aspect-video">
          <iframe 
            width="100%" 
            height="100%" 
            src="https://www.youtube.com/embed/9p800T0LhB4" 
            title="Da Lucrezia al codice rosso" 
            frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
            referrerpolicy="strict-origin-when-cross-origin" 
            allowfullscreen
            class="rounded-xl"
          ></iframe>
        </div>
      </div>
      
      <p class="text-gray-700 leading-relaxed">
        La violenza di genere non è una questione privata, né può essere lasciata sulle spalle delle sole vittime. È una responsabilità collettiva che coinvolge istituzioni, famiglie, scuole, media e ogni cittadino. Solo con una visione condivisa e con azioni concrete – dalla legge alla cultura, dalla scuola ai tribunali – possiamo sperare di costruire una società più giusta, dove nessuna donna debba più avere paura di tornare a casa, amare, parlare, esistere.
      </p>
      
      <blockquote class="border-l-4 border-pink-500 pl-6 italic text-lg text-gray-700 mt-8">
        "Il silenzio è complice della violenza. Parlare, denunciare e agire sono i nostri strumenti per spezzare le catene dell'oppressione."
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
