<script>
  let expandedId = null;
  
  function toggleExpand(id) {
    expandedId = expandedId === id ? null : id;
  }
</script>

<div class="max-w-4xl mx-auto">
  <div class="text-center mb-12">
    <h1 class="text-4xl font-bold text-gray-900 mb-4">PCTO</h1>
    <p class="text-xl text-gray-600">
      Percorsi per le Competenze Trasversali e per l'Orientamento
    </p>
  </div>

  <div class="bg-white rounded-lg shadow-sm border border-gray-200 p-8 mb-8">
    <h2 class="text-2xl font-semibold mb-4">Panoramica del Percorso</h2>
    <p class="text-gray-600 mb-6">
      Il percorso PCTO ha rappresentato un'opportunità fondamentale per sviluppare competenze trasversali 
      e acquisire una maggiore consapevolezza del mondo del lavoro, con particolare focus sui temi di 
      educazione civica e cittadinanza attiva.
    </p>
    
    <div class="grid md:grid-cols-3 gap-6">
      <div class="text-center">
        <div class="bg-blue-100 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-3">
          <span class="text-2xl">⏱️</span>
        </div>
        <h3 class="font-semibold mb-2">Ore Totali</h3>
        <p class="text-gray-600">+150 ore</p>
      </div>
      
      <div class="text-center">
        <div class="bg-green-100 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-3">
          <span class="text-2xl">🏢</span>
        </div>
        <h3 class="font-semibold mb-2">Enti Partner</h3>
        <p class="text-gray-600">2 organizzazioni</p>
      </div>
    </div>
  </div>

  <div class="space-y-8">
    <h2 class="text-2xl font-semibold">Esperienze Formative</h2>
    
    <div class="bg-white rounded-lg shadow-sm border border-gray-200 p-6 transition-all duration-300">
      <div class="flex items-start justify-between mb-4">
        <div>
          <h3 class="text-xl font-semibold text-gray-900">Stage estivo presso: EasyNet Srl.</h3>
          <p class="text-gray-600">Azienda di consulenza informatica</p>
        </div>
        <span class="bg-blue-100 text-blue-800 text-sm font-medium px-3 py-1 rounded">100 ore</span>
      </div>
      
      <p class="text-gray-600 mb-4">
        Sviluppo applicazioni con tecnologie .Net
      </p>
      
      <button 
        class="text-blue-600 hover:text-blue-800 font-medium flex items-center gap-1"
        on:click={() => toggleExpand('easynet')}
      >
        {expandedId === 'easynet' ? 'Mostra meno' : 'Leggi di più'}
        <svg class="w-4 h-4 transition-transform {expandedId === 'easynet' ? 'rotate-180' : ''}" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path>
        </svg>
      </button>
      
      {#if expandedId === 'easynet'}
        <div class="mt-4 pt-4 border-t border-gray-100 text-gray-700 space-y-3 transition-all">
          <p>
            Durante questo stage estivo ho avuto l'opportunità di lavorare in un ambiente professionale dinamico, collaborando con un team di sviluppatori esperti nella creazione di soluzioni software personalizzate per clienti aziendali.
          </p>
          <p>
            <strong>Attività principali:</strong>
          </p>
          <ul class="list-disc pl-5 space-y-1">
            <li>Sviluppo di applicazioni web utilizzando tecnologie HTML/CSS/JS</li>
            <li>Implementazione di interfacce utente responsive con HTML, CSS e JavaScript</li>
            <li>Partecipazione a riunioni di team e sessioni di pianificazione dei progetti</li>
            <li>Testing e debugging del codice</li>
          </ul>
          <p>
            <strong>Competenze acquisite:</strong>
          </p>
          <ul class="list-disc pl-5 space-y-1">
            <li>Comprensione del ciclo di sviluppo software in ambiente aziendale</li>
            <li>Capacità di lavoro in team e comunicazione tecnica</li>
            <li>Approccio strutturato alla risoluzione dei problemi</li>
            <li>Gestione efficiente del tempo e delle priorità</li>
          </ul>
          <p>
            Questa esperienza mi ha permesso di applicare in contesti reali le conoscenze teoriche acquisite a scuola, confrontandomi con le sfide concrete dello sviluppo software professionale.
          </p>
        </div>
      {/if}
      
      <div class="border-t pt-4 mt-4">
        <p class="text-sm text-gray-500">Periodo: Giugno - Luglio 2023</p>
      </div>
    </div>

    <div class="bg-white rounded-lg shadow-sm border border-gray-200 p-6">
      <div class="flex items-start justify-between mb-4">
        <div>
          <h3 class="text-xl font-semibold text-gray-900">Progetto Find My Tutor</h3>
          <p class="text-gray-600">Gestione della piattaforma</p>
        </div>
        <span class="bg-green-100 text-green-800 text-sm font-medium px-3 py-1 rounded">50 ore</span>
      </div>
      
      <p class="text-gray-600 mb-4">
        Gestione della piattaforma e implementazione di nuove funzionalità
      </p>
      
      <button 
        class="text-blue-600 hover:text-blue-800 font-medium flex items-center gap-1"
        on:click={() => toggleExpand('findmytutor')}
      >
        {expandedId === 'findmytutor' ? 'Mostra meno' : 'Leggi di più'}
        <svg class="w-4 h-4 transition-transform {expandedId === 'findmytutor' ? 'rotate-180' : ''}" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path>
        </svg>
      </button>
      
      {#if expandedId === 'findmytutor'}
        <div class="mt-4 pt-4 border-t border-gray-100 text-gray-700 space-y-3 transition-all">
          <p>
            "Find My Tutor" è una piattaforma innovativa sviluppata all'interno dell'istituto per facilitare l'incontro tra studenti che necessitano di supporto didattico e compagni più esperti disponibili a offrire tutoraggio.
          </p>
          <p>
            <strong>Il mio contributo al progetto:</strong>
          </p>
          <ul class="list-disc pl-5 space-y-1">
            <li>Progettazione e implementazione del sistema di matching tra studenti e tutor</li>
            <li>Creazione di un'interfaccia utente intuitiva con Wordpress</li>
            <li>Implementazione di un sistema di notifiche via email</li>
            <li>Ottimizzazione delle prestazioni della piattaforma</li>
          </ul>
          <p>
            <strong>Obiettivi del progetto:</strong>
          </p>
          <ul class="list-disc pl-5 space-y-1">
            <li>Promuovere la collaborazione tra pari e il peer learning</li>
            <li>Valorizzare le competenze degli studenti più preparati</li>
            <li>Creare uno strumento digitale utile alla comunità scolastica</li>
            <li>Sviluppare competenze tecniche e soft skills nei partecipanti</li>
          </ul>
          <p>
            La piattaforma è stata adottata con successo dall'istituto e ha registrato oltre 200 sessioni di, ricevendo feedback molto positivi sia dagli studenti che dai docenti coordinatori.
          </p>
        </div>
      {/if}
      
      <div class="border-t pt-4 mt-4">
        <p class="text-sm text-gray-500">Periodo: Settembre 2024 - Giugno 2025</p>
      </div>
    </div>
  </div>
</div>

<style>
  /* Optional: Add animation for smooth transitions */
  .transition-all {
    transition-property: all;
    transition-duration: 300ms;
  }
</style>