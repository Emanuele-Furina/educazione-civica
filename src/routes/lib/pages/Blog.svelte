<script>
  import { base } from "$app/paths";

  const articles = [
    {
      id: "pena-di-morte",
      title: "La pena di morte e l'umanità del condannato",
      excerpt:
        "Un viaggio tra letteratura e realtà, attraverso la riflessione sulla pena di morte e il capolavoro di Victor Hugo, 'L'ultimo giorno di un condannato a morte'.",
      date: "29 Dicembre 2022",
      category: "Letteratura",
      readTime: "12 min",
      image: `${base}/images/sedia-elettrica.jpeg`,
    },
    {
      id: "storia-mafia",
      title: "La Storia della Mafia e le Stragi",
      excerpt:
        "Un approfondito viaggio attraverso la storia della mafia italiana, dalle origini ottocentesche alle stragi degli anni '90, per comprendere e non dimenticare chi ha sacrificato la vita per la legalità.",
      date: "22 Marzo 2022",
      category: "Storia",
      readTime: "15 min",
      image: `${base}/images/falcone.jpeg`,
    },
    {
      id: "violenza-genere",
      title: "La violenza di genere e i femminicidi",
      excerpt:
        "Un'analisi del fenomeno della violenza di genere tra storia, società e dati, per comprendere meglio una delle più gravi emergenze sociali del nostro tempo.",
      date: "30 Novembre 2022",
      category: "Società",
      readTime: "10 min",
      image: `${base}/images/violenza_donne.jpg`,
    },
    {
      id: "war-poetry",
      title: "War Poetry - Voices from the Battlefield",
      excerpt:
        "An analysis of war poetry through the lens of Rupert Brooke's 'The Soldier', Wilfred Owen's 'Dulce et Decorum Est', and W.H. Auden's 'Refugee Blues'.",
      date: "27 Maggio 2025",
      category: "Letteratura",
      readTime: "8 min",
      image: `${base}/images/war-poetry.jpg`,
    },
    {
      id: "carcere-speranza",
      title: "Carcere e speranza",
      excerpt:
        "Un viaggio nella realtà del carcere tra teatro, speranza e rieducazione. Esperienze e riflessioni che interrogano la società attraverso lo spettacolo 'Le Finestre'.",
      date: "27 Marzo 2023",
      category: "Società",
      readTime: "9 min",
      image: `${base}/images/carcere.png`,
    },
  ];

  const categories = ["Tutti", "Letteratura", "Storia", "Società"];
  let selectedCategory = $state("Tutti");
  let { navigateTo } = $props();

  const filteredArticles = $derived(
    selectedCategory === "Tutti"
      ? articles
      : articles.filter((article) => article.category === selectedCategory),
  );
</script>

<div class="max-w-6xl mx-auto">
  <div class="text-center mb-16 relative">
    <div
      class="absolute top-0 left-1/2 transform -translate-x-1/2 -translate-y-4 w-24 h-1 bg-gradient-to-r from-blue-500 to-purple-500 rounded-full"
    ></div>

    <h1 class="text-5xl font-bold mb-6">
      <span
        class="bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent"
      >
        Blog di Educazione Civica
      </span>
    </h1>
    <p class="text-xl text-gray-600 max-w-3xl mx-auto leading-relaxed">
      Articoli, riflessioni e approfondimenti sui temi fondamentali della
      cittadinanza
    </p>
  </div>

  <div class="flex flex-wrap justify-center gap-3 mb-16">
    {#each categories as category}
      <button
        onclick={() => (selectedCategory = category)}
        class="px-6 py-3 rounded-2xl text-sm font-semibold transition-all duration-300 transform hover:scale-105
               {selectedCategory === category
          ? 'bg-gradient-to-r from-blue-500 to-purple-500 text-white shadow-lg shadow-blue-500/25'
          : 'bg-white/70 backdrop-blur-sm text-gray-700 hover:bg-white hover:shadow-md border border-white/50'}"
      >
        {category}
      </button>
    {/each}
  </div>

  <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
    {#each filteredArticles as article}
      <article
        class="group bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 overflow-hidden hover:shadow-2xl transition-all duration-500 transform hover:scale-105"
      >
        <div class="relative overflow-hidden">
          <img
            src={article.image || `${base}/images/placeholder.svg`}
            alt={article.title}
            class="w-full h-48 object-cover group-hover:scale-110 transition-transform duration-500"
          />
          <div
            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"
          ></div>
        </div>

        <div class="p-6">
          <div class="flex items-center justify-between mb-4">
            <span
              class="bg-gradient-to-r from-blue-500 to-purple-500 text-white text-xs font-bold px-3 py-1 rounded-full shadow-lg"
            >
              {article.category}
            </span>
            <span
              class="text-gray-500 text-sm bg-gray-100 px-2 py-1 rounded-full"
              >{article.readTime}</span
            >
          </div>

          <h2
            class="text-xl font-bold text-gray-900 mb-3 line-clamp-2 group-hover:text-blue-600 transition-colors duration-300"
          >
            {article.title}
          </h2>

          <p class="text-gray-600 text-sm mb-4 line-clamp-3 leading-relaxed">
            {article.excerpt}
          </p>

          <div class="flex items-center justify-between">
            <span class="text-gray-500 text-sm">{article.date}</span>
            <button
              onclick={() => navigateTo(article.id)}
              class="flex items-center text-blue-600 hover:text-blue-800 text-sm font-semibold group-hover:translate-x-1 transition-all duration-300"
            >
              <span>Leggi tutto</span>
              <svg
                class="w-4 h-4 ml-1"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M9 5l7 7-7 7"
                ></path>
              </svg>
            </button>
          </div>
        </div>
      </article>
    {/each}
  </div>

  {#if filteredArticles.length === 0}
    <div class="text-center py-16">
      <div class="text-6xl mb-4">📝</div>
      <p class="text-gray-500 text-xl">
        Nessun articolo trovato per questa categoria.
      </p>
    </div>
  {/if}
</div>
