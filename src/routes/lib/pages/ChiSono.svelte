<script>
  import { base } from "$app/paths";
</script>

<div class="max-w-4xl mx-auto">
  <div class="text-center mb-16 relative">
    <div class="absolute inset-0 -z-10">
      <div class="absolute top-10 left-10 w-32 h-32 bg-blue-300 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-pulse"></div>
      <div class="absolute top-20 right-10 w-32 h-32 bg-purple-300 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-pulse animation-delay-1000"></div>
    </div>

    <div class="relative">
      <div class="w-40 h-40 bg-gradient-to-br from-blue-400 via-purple-500 to-pink-500 rounded-full mx-auto mb-8 flex items-center justify-center shadow-2xl shadow-blue-500/25 animate-bounce-slow overflow-hidden">
        <img src="{base}/images/me.jpg" alt="" class="w-full h-full object-cover rounded-full">
      </div>
      
      <h1 class="text-5xl font-bold mb-4">
        <span class="bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
          Emanuele Furina
        </span>
      </h1>
      <p class="text-xl text-gray-600 leading-relaxed">
        Studente del 5° anno
      </p>
    </div>
  </div>


  <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 mb-8 hover:shadow-2xl transition-all duration-500">
    <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">Chi Sono</h2>
    <div class="prose prose-gray max-w-none">
      <p class="text-gray-600 mb-4 leading-relaxed text-lg">
        Sono Emanuele Furina, uno studente del quinto anno con una grande passione per lo sviluppo 
        software e le tecnologie moderne. Il mio percorso di studi mi ha portato ad approfondire 
        non solo gli aspetti tecnici dell'informatica, ma anche i temi fondamentali dell'educazione 
        civica e della cittadinanza digitale.
      </p>
    </div>
  </div>

  <div class="grid md:grid-cols-2 gap-8 mb-8">
    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 hover:shadow-2xl transition-all duration-500 transform hover:scale-105">
      <h3 class="text-2xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">Competenze Tecniche</h3>
      <div class="space-y-4">
        <div class="flex items-center justify-between">
          <span class="text-gray-700 font-medium">Sviluppo Lua</span>
          <div class="flex space-x-1">
            {#each Array(5) as _, i}
              <div class="w-3 h-3 rounded-full transition-all duration-300 {i < 4 ? 'bg-gradient-to-r from-blue-500 to-purple-500 shadow-lg' : 'bg-gray-200'}"></div>
            {/each}
          </div>
        </div>
        <div class="flex items-center justify-between">
          <span class="text-gray-700 font-medium">JavaScript</span>
          <div class="flex space-x-1">
            {#each Array(5) as _, i}
              <div class="w-3 h-3 rounded-full transition-all duration-300 {i < 4 ? 'bg-gradient-to-r from-green-500 to-blue-500 shadow-lg' : 'bg-gray-200'}"></div>
            {/each}
          </div>
        </div>
        <div class="flex items-center justify-between">
          <span class="text-gray-700 font-medium">Svelte</span>
          <div class="flex space-x-1">
            {#each Array(5) as _, i}
              <div class="w-3 h-3 rounded-full transition-all duration-300 {i < 3 ? 'bg-gradient-to-r from-purple-500 to-pink-500 shadow-lg' : 'bg-gray-200'}"></div>
            {/each}
          </div>
        </div>
        <div class="flex items-center justify-between">
          <span class="text-gray-700 font-medium">Progettazione Database</span>
          <div class="flex space-x-1">
            {#each Array(5) as _, i}
              <div class="w-3 h-3 rounded-full transition-all duration-300 {i < 3 ? 'bg-gradient-to-r from-orange-500 to-red-500 shadow-lg' : 'bg-gray-200'}"></div>
            {/each}
          </div>
        </div>
      </div>
    </div>
  <div class="bg-white rounded-lg shadow-sm border border-gray-200 p-8 mb-8">
    <h2 class="text-2xl font-semibold mb-6">Percorso Formativo</h2>
    <div class="space-y-6">
      <div class="border-l-4 border-blue-500 pl-6">
        <h3 class="text-lg font-semibold text-gray-900">Diploma di Maturità</h3>
        <p class="text-gray-600">Istituto Tecnico Informatico - 2025</p>
        <p class="text-sm text-gray-500 mt-2">
          Specializzazione in informatica con approfondimenti in educazione civica e cittadinanza digitale
        </p>
      </div>

    </div>
  </div>

  <div class="bg-gradient-to-r from-blue-50 to-purple-50 rounded-lg p-8">
    <h2 class="text-2xl font-semibold mb-6">Obiettivi Futuri</h2>
    <div class="grid md:grid-cols-2 gap-6">
      <div>
        <h3 class="text-lg font-semibold mb-3">Professionali</h3>
        <ul class="space-y-2 text-gray-700">
          <li class="flex items-center space-x-2">
            <span class="text-green-500">✓</span>
            <span>Laurea in Informatica</span>
          </li>
          <li class="flex items-center space-x-2">
            <span class="text-green-500">✓</span>
            <span>Specializzazione in Cybersecurity o Forensica digitale</span>
          </li>
        </ul>
      </div>
      
      <div>
        <h3 class="text-lg font-semibold mb-3">Personali</h3>
        <ul class="space-y-2 text-gray-700">
          <li class="flex items-center space-x-2">
            <span class="text-green-500">✓</span>
            <span>Contribuire a progetti open source</span>
          </li>
          <li class="flex items-center space-x-2">
            <span class="text-green-500">✓</span>
            <span>Promuovere la cittadinanza digitale</span>
          </li>
          <li class="flex items-center space-x-2">
            <span class="text-green-500">✓</span>
            <span>Partecipazione attiva nella comunità</span>
          </li>
        </ul>
      </div>
    </div>
  </div>

  </div>
</div>

<style>
  @keyframes bounce-slow {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
  }
  
  .animate-bounce-slow { animation: bounce-slow 3s ease-in-out infinite; }
  .animation-delay-1000 { animation-delay: 1s; }
</style>
