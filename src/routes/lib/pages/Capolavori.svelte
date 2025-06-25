<script>
  let { navigateTo } = $props();
  import { base } from "$app/paths";
  const masterpieces = [
    {
      id: 1,
      title: "Creazione e Gesitone server FiveM",
      type: "Informatica",
      description: "Creazione, programmazione e gestione di un server RP",
      date: "2023-2025",
      image: `${base}/images/fivem.png`,
      tags: ["Informatica", "Programmazione", "Giochi"],
      link: "fivem"
    },
    {
      id: 2,
      title: "Piattaforma Find My Tutor",
      type: "Sociale",
      description: "Gestione della piattaforma Find My Tutor",
      date: "2024-2025",
      image: `${base}/images/find.jpg`,
      tags: ["Digitale","Innovazione"],
      link: "https://findmytutor.agnelli.it"
    }
  ];

  const types = ["Tutti", "Informatica", "Sociale"];
  let selectedType = $state("Tutti");

  const filteredMasterpieces = $derived(
    selectedType === "Tutti" 
      ? masterpieces 
      : masterpieces.filter(item => item.type === selectedType)
  );

  // @ts-ignore
  function openProject(link) {
    if (link && link !== "#") {
      if (link.startsWith('http')) {
        window.open(link, '_blank');
      } else {
        navigateTo(link);
      }
    }
  }
</script>

<div class="max-w-6xl mx-auto">
  <div class="text-center mb-12">
    <h1 class="text-4xl font-bold text-gray-900 mb-4">Capolavori</h1>
    <p class="text-xl text-gray-600 max-w-2xl mx-auto">
      Una raccolta dei migliori lavori e progetti realizzati durante il percorso di educazione civica
    </p>
  </div>

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

  <div class="flex flex-wrap justify-center gap-8">
    {#each filteredMasterpieces as item}
      <div class="bg-white rounded-lg shadow-sm border border-gray-200 overflow-hidden hover:shadow-md transition-shadow w-full max-w-sm">
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
          
          <button 
            onclick={() => openProject(item.link)}
            class="w-full bg-blue-600 text-white py-2 px-4 rounded-md hover:bg-blue-700 transition-colors text-sm font-medium
                   {item.link === '#' ? 'opacity-50 cursor-not-allowed' : 'cursor-pointer'}"
            disabled={item.link === '#'}
          >
            {item.link === '#' ? 'Progetto Non Disponibile' : 'Visualizza Progetto'}
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
</div>