<script>
  const masterpieces = [
    {
      id: 1,
      title: "Analisi Comparativa delle Costituzioni Europee",
      type: "Ricerca",
      description: "Studio approfondito che confronta i principi fondamentali delle costituzioni di Italia, Francia, Germania e Spagna, evidenziando similitudini e differenze nell'approccio ai diritti fondamentali.",
      date: "Marzo 2024",
      image: "/placeholder.svg?height=300&width=400",
      tags: ["Costituzione", "Europa", "Diritti"],
      link: "#"
    },
    {
      id: 2,
      title: "Progetto Multimediale: La Cittadinanza Digitale",
      type: "Progetto Multimediale",
      description: "Creazione di un sito web interattivo e di video informativi sui rischi e le opportunità del mondo digitale, con focus su privacy, fake news e partecipazione democratica online.",
      date: "Febbraio 2024",
      image: "/placeholder.svg?height=300&width=400",
      tags: ["Digitale", "Media", "Partecipazione"],
      link: "#"
    },
    {
      id: 3,
      title: "Saggio: L'Evoluzione del Concetto di Cittadinanza",
      type: "Saggio",
      description: "Elaborato che traccia l'evoluzione storica del concetto di cittadinanza dall'antica Grecia ai giorni nostri, con particolare attenzione alle sfide della globalizzazione.",
      date: "Gennaio 2024",
      image: "/placeholder.svg?height=300&width=400",
      tags: ["Storia", "Filosofia", "Globalizzazione"],
      link: "#"
    },
    {
      id: 4,
      title: "Presentazione: Agenda 2030 e Sviluppo Sostenibile",
      type: "Presentazione",
      description: "Presentazione interattiva sui 17 obiettivi dell'Agenda 2030 dell'ONU, con analisi delle politiche italiane ed europee per lo sviluppo sostenibile.",
      date: "Dicembre 2023",
      image: "/placeholder.svg?height=300&width=400",
      tags: ["Sostenibilità", "ONU", "Ambiente"],
      link: "#"
    },
    {
      id: 5,
      title: "Podcast: Voci della Democrazia",
      type: "Podcast",
      description: "Serie di episodi podcast che esplorano temi democratici attraverso interviste a esperti, cittadini e rappresentanti delle istituzioni locali.",
      date: "Novembre 2023",
      image: "/placeholder.svg?height=300&width=400",
      tags: ["Audio", "Democrazia", "Interviste"],
      link: "#"
    },
    {
      id: 6,
      title: "Infografica: Il Sistema Elettorale Italiano",
      type: "Infografica",
      description: "Rappresentazione visuale del complesso sistema elettorale italiano, dalle elezioni politiche a quelle amministrative, con spiegazioni chiare e accessibili.",
      date: "Ottobre 2023",
      image: "/placeholder.svg?height=300&width=400",
      tags: ["Elezioni", "Grafica", "Sistema politico"],
      link: "#"
    }
  ];

  const types = ["Tutti", "Ricerca", "Progetto Multimediale", "Saggio", "Presentazione", "Podcast", "Infografica"];
  let selectedType = $state("Tutti");

  const filteredMasterpieces = $derived(
    selectedType === "Tutti" 
      ? masterpieces 
      : masterpieces.filter(item => item.type === selectedType)
  );
</script>

<div class="max-w-6xl mx-auto">
  <div class="text-center mb-12">
    <h1 class="text-4xl font-bold text-gray-900 mb-4">Capolavori</h1>
    <p class="text-xl text-gray-600 max-w-2xl mx-auto">
      Una raccolta dei migliori lavori e progetti realizzati durante il percorso di educazione civica
    </p>
  </div>

  <!-- Type Filter -->
  <div class="flex flex-wrap justify-center gap-2 mb-12">
    {#each types as type}
      <button
        onclick={() => selectedType = type}
        class="px-4 py-2 rounded-full text-sm font-medium transition-colors
               {selectedType === type 
                 ? 'bg-blue-600 text-white' 
                 : 'bg-gray-100 text-gray-700 hover:bg-gray-200'}"
      >
        {type}
      </button>
    {/each}
  </div>

  <!-- Masterpieces Grid -->
  <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
    {#each filteredMasterpieces as item}
      <div class="bg-white rounded-lg shadow-sm border border-gray-200 overflow-hidden hover:shadow-md transition-shadow">
        <img 
          src={item.image || "/placeholder.svg"} 
          alt={item.title}
          class="w-full h-48 object-cover"
        />
        <div class="p-6">
          <div class="flex items-center justify-between mb-3">
            <span class="bg-purple-100 text-purple-800 text-xs font-medium px-2.5 py-0.5 rounded">
              {item.type}
            </span>
            <span class="text-gray-500 text-sm">{item.date}</span>
          </div>
          
          <h3 class="text-xl font-semibold text-gray-900 mb-3 line-clamp-2">
            {item.title}
          </h3>
          
          <p class="text-gray-600 text-sm mb-4 line-clamp-3">
            {item.description}
          </p>
          
          <div class="flex flex-wrap gap-1 mb-4">
            {#each item.tags as tag}
              <span class="bg-gray-100 text-gray-700 text-xs px-2 py-1 rounded">
                {tag}
              </span>
            {/each}
          </div>
          
          <button class="w-full bg-blue-600 text-white py-2 px-4 rounded-md hover:bg-blue-700 transition-colors text-sm font-medium">
            Visualizza Progetto
          </button>
        </div>
      </div>
    {/each}
  </div>

  {#if filteredMasterpieces.length === 0}
    <div class="text-center py-12">
      <p class="text-gray-500 text-lg">Nessun capolavoro trovato per questa categoria.</p>
    </div>
  {/if}

  <!-- Achievement Stats -->
  <div class="bg-gradient-to-r from-blue-50 to-purple-50 rounded-lg p-8 mt-16">
    <h2 class="text-2xl font-semibold text-center mb-8">Risultati Raggiunti</h2>
    <div class="grid md:grid-cols-4 gap-6 text-center">
      <div>
        <div class="text-3xl font-bold text-blue-600 mb-2">6</div>
        <p class="text-gray-600">Progetti Completati</p>
      </div>
      <div>
        <div class="text-3xl font-bold text-green-600 mb-2">15</div>
        <p class="text-gray-600">Competenze Sviluppate</p>
      </div>
      <div>
        <div class="text-3xl font-bold text-purple-600 mb-2">4</div>
        <p class="text-gray-600">Tipologie di Media</p>
      </div>
      <div>
        <div class="text-3xl font-bold text-orange-600 mb-2">100+</div>
        <p class="text-gray-600">Ore di Lavoro</p>
      </div>
    </div>
  </div>
</div>
