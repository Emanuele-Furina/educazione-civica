<script>
  let { navigateTo } = $props();
</script>

<div class="max-w-6xl mx-auto">

  <div class="text-center py-20 relative overflow-hidden">

    <div class="absolute inset-0 -z-10">
      <div
        class="absolute top-20 left-10 w-72 h-72 bg-blue-300 rounded-full mix-blend-multiply filter blur-xl opacity-30 animate-blob"
      ></div>
      <div
        class="absolute top-40 right-10 w-72 h-72 bg-purple-300 rounded-full mix-blend-multiply filter blur-xl opacity-30 animate-blob animation-delay-2000"
      ></div>
      <div
        class="absolute -bottom-8 left-20 w-72 h-72 bg-pink-300 rounded-full mix-blend-multiply filter blur-xl opacity-30 animate-blob animation-delay-4000"
      ></div>
    </div>

    <div class="relative z-10">
      <div
        class="inline-block p-4 bg-white/20 backdrop-blur-sm rounded-full mb-6 animate-bounce-slow"
      >
        <span class="text-6xl">🎓</span>
      </div>

      <h1 class="text-5xl md:text-7xl font-bold mb-6 animate-fade-in-up">
        <span
          class="bg-gradient-to-r from-blue-600 via-purple-600 to-pink-600 bg-clip-text text-transparent"
        >
          Educazione
        </span>
        <br />
        <span
          class="bg-gradient-to-r from-purple-600 via-pink-600 to-red-500 bg-clip-text text-transparent"
        >
          Civica
        </span>
      </h1>

      <p
        class="text-xl md:text-2xl text-gray-600 mb-8 max-w-3xl mx-auto leading-relaxed animate-fade-in-up animation-delay-300"
      >
        Portfolio digitale per il 5° anno<br />
        <span
          class="font-semibold bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent"
        >
          Un percorso attraverso cittadinanza, diritti e doveri civici
        </span>
      </p>

      <div
        class="f lex flex-col sm:flex-row gap-4 justify-center animate-fade-in-up animation-delay-600"
      >
        <button
          onclick={() => navigateTo("blog")}
          class="group bg-gradient-to-r from-blue-500 to-purple-600 text-white px-8 py-4 rounded-2xl font-semibold hover:shadow-2xl hover:shadow-blue-500/25 transition-all duration-300 transform hover:scale-105"
        >
          <span class="flex items-center space-x-2">
            <span>Esplora i Contenuti</span>
            <svg
              class="w-5 h-5 group-hover:translate-x-1 transition-transform duration-300"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M13 7l5 5m0 0l-5 5m5-5H6"
              ></path>
            </svg>
          </span>
        </button>
        <button
          onclick={() => navigateTo("chi-sono")}
          class="group bg-white/80 backdrop-blur-sm text-gray-700 px-8 py-4 rounded-2xl font-semibold hover:bg-white hover:shadow-xl transition-all duration-300 transform hover:scale-105 border border-white/50"
        >
          <span class="flex items-center space-x-2">
            <span>Scopri di Più</span>
            <svg
              class="w-5 h-5 group-hover:rotate-12 transition-transform duration-300"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
              ></path>
            </svg>
          </span>
        </button>
      </div>
    </div>
  </div>


  <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6 py-16">
    <div
      class="group text-center p-8 bg-white/60 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 hover:bg-white/80 transition-all duration-500 transform hover:scale-105 hover:shadow-2xl"
    >
      <div
        class="text-5xl mb-6 group-hover:scale-110 transition-transform duration-300"
      >
        📝
      </div>
      <h3
        class="text-xl font-bold mb-3 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent"
      >
        Articoli Blog
      </h3>
      <p class="text-gray-600 text-sm leading-relaxed">
        Riflessioni e approfondimenti sui temi di educazione civica
      </p>
    </div>

    <div
      class="group text-center p-8 bg-white/60 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 hover:bg-white/80 transition-all duration-500 transform hover:scale-105 hover:shadow-2xl"
    >
      <div
        class="text-5xl mb-6 group-hover:scale-110 transition-transform duration-300"
      >
        💼
      </div>
      <h3
        class="text-xl font-bold mb-3 bg-gradient-to-r from-green-600 to-blue-600 bg-clip-text text-transparent"
      >
        PCTO
      </h3>
      <p class="text-gray-600 text-sm leading-relaxed">
        Percorsi per le Competenze Trasversali e l'Orientamento
      </p>
    </div>

    <div
      class="group text-center p-8 bg-white/60 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 hover:bg-white/80 transition-all duration-500 transform hover:scale-105 hover:shadow-2xl"
    >
      <div
        class="text-5xl mb-6 group-hover:scale-110 transition-transform duration-300"
      >
        🎨
      </div>
      <h3
        class="text-xl font-bold mb-3 bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent"
      >
        Capolavori
      </h3>
      <p class="text-gray-600 text-sm leading-relaxed">
        I migliori lavori e progetti realizzati durante l'anno
      </p>
    </div>

    <div
      class="group text-center p-8 bg-white/60 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 hover:bg-white/80 transition-all duration-500 transform hover:scale-105 hover:shadow-2xl"
    >
      <div
        class="text-5xl mb-6 group-hover:scale-110 transition-transform duration-300"
      >
        👤
      </div>
      <h3
        class="text-xl font-bold mb-3 bg-gradient-to-r from-orange-600 to-red-600 bg-clip-text text-transparent"
      >
        Chi Sono
      </h3>
      <p class="text-gray-600 text-sm leading-relaxed">
        Presentazione personale e percorso formativo
      </p>
    </div>
  </div>
</div>

<style>
  @keyframes blob {
    0% {
      transform: translate(0px, 0px) scale(1);
    }
    33% {
      transform: translate(30px, -50px) scale(1.1);
    }
    66% {
      transform: translate(-20px, 20px) scale(0.9);
    }
    100% {
      transform: translate(0px, 0px) scale(1);
    }
  }

  @keyframes fade-in-up {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @keyframes bounce-slow {
    0%,
    100% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-10px);
    }
  }

  .animate-blob {
    animation: blob 7s infinite;
  }
  .animate-fade-in-up {
    animation: fade-in-up 0.8s ease-out;
  }
  .animate-bounce-slow {
    animation: bounce-slow 3s ease-in-out infinite;
  }
  .animation-delay-300 {
    animation-delay: 0.3s;
  }
  .animation-delay-600 {
    animation-delay: 0.6s;
  }
  .animation-delay-2000 {
    animation-delay: 2s;
  }
  .animation-delay-4000 {
    animation-delay: 4s;
  }
</style>
