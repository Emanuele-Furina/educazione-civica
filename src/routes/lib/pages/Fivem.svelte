<script>
  let { navigateTo } = $props();
</script>

<div class="max-w-6xl mx-auto">
  <div class="text-center mb-16 relative">
    <div class="absolute inset-0 -z-10">
      <div class="absolute top-10 left-20 w-64 h-64 bg-purple-300 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-pulse"></div>
      <div class="absolute top-20 right-20 w-64 h-64 bg-blue-300 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-pulse animation-delay-1000"></div>
    </div>

    <div class="relative">
      <div class="mb-8">
        <span class="bg-gradient-to-r from-purple-500 to-blue-500 text-white text-sm font-bold px-4 py-2 rounded-full shadow-lg">
          🎮 Progetto Gaming
        </span>
      </div>
      
      <h1 class="text-5xl font-bold mb-6">
        <span class="bg-gradient-to-r from-purple-600 to-blue-600 bg-clip-text text-transparent">
          Liberty RP Server
        </span>
      </h1>
      
      <p class="text-xl text-gray-600 max-w-4xl mx-auto leading-relaxed mb-8">
        Un viaggio nella creazione e gestione di un server FiveM RP: quando la passione per il gaming incontra la programmazione e nasce una comunità virtuale
      </p>

      <div class="flex items-center justify-center space-x-6 text-sm text-gray-500">
        <span class="flex items-center space-x-2">
          <span>📅</span>
          <span>2023 - 2025</span>
        </span>
        <span class="flex items-center space-x-2">
          <span>👥</span>
          <span>Progetto di Gruppo</span>
        </span>
        <span class="flex items-center space-x-2">
          <span>💻</span>
          <span>Lua, MySQL, HTML/CSS/JS</span>
        </span>
      </div>
    </div>
  </div>


  <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 mb-8">
    <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-purple-600 to-blue-600 bg-clip-text text-transparent">
      Dall'idea alla realtà virtuale
    </h2>
    
    <p class="text-gray-700 leading-relaxed mb-6">
      Tutto è iniziato con una semplice domanda: <strong>"E se potessimo creare il nostro mondo?"</strong> Era il 2023 quando, insieme ad alcuni amici appassionati di gaming, abbiamo deciso di lanciarci nell'avventura di creare un server FiveM RP personalizzato. Non sapevamo ancora che questa esperienza sarebbe diventata una vera e propria scuola di programmazione, gestione e leadership.
    </p>
    
    <p class="text-gray-700 leading-relaxed">
      <strong>Liberty RP</strong> non è nato come un semplice server di gioco, ma come un progetto ambizioso: creare una comunità virtuale dove ogni giocatore potesse vivere una "seconda vita" digitale, assumendo ruoli, professioni e storie uniche in un ambiente realistico e coinvolgente basato su Grand Theft Auto V.
    </p>
  </div>

  <div class="grid md:grid-cols-2 gap-8 mb-8">
    <div class="bg-gradient-to-br from-blue-50 to-purple-50 rounded-3xl p-8 border border-blue-200">
      <h3 class="text-2xl font-bold mb-6 text-blue-800">
        🔧 Architettura Tecnica
      </h3>
      
      <div class="space-y-4">
        <div class="bg-white/70 p-4 rounded-xl">
          <h4 class="font-semibold text-blue-700 mb-2">Backend - Lua Scripting</h4>
          <p class="text-sm text-gray-600">Framework ESX per gestione economia, lavori, inventari e meccaniche di gioco</p>
        </div>
        
        <div class="bg-white/70 p-4 rounded-xl">
          <h4 class="font-semibold text-blue-700 mb-2">Database - MySQL</h4>
          <p class="text-sm text-gray-600">Persistenza dati giocatori, proprietà, transazioni e statistiche server</p>
        </div>
        
        <div class="bg-white/70 p-4 rounded-xl">
          <h4 class="font-semibold text-blue-700 mb-2">Frontend - Web UI</h4>
          <p class="text-sm text-gray-600">Interfacce HTML/CSS/JS per inventari, menu e pannelli di controllo</p>
        </div>
      </div>
    </div>

    <div class="bg-gradient-to-br from-purple-50 to-pink-50 rounded-3xl p-8 border border-purple-200">
      <h3 class="text-2xl font-bold mb-6 text-purple-800">
        📊 Numeri del Progetto
      </h3>
      
      <div class="grid grid-cols-2 gap-4">
        <div class="text-center bg-white/70 p-4 rounded-xl">
          <div class="text-2xl font-bold text-purple-600">50+</div>
          <div class="text-sm text-gray-600">Script Personalizzati</div>
        </div>
        
        <div class="text-center bg-white/70 p-4 rounded-xl">
          <div class="text-2xl font-bold text-purple-600">24/7</div>
          <div class="text-sm text-gray-600">Server Operativo</div>
        </div>
        
        <div class="text-center bg-white/70 p-4 rounded-xl">
          <div class="text-2xl font-bold text-purple-600">Team</div>
          <div class="text-sm text-gray-600">Collaborativo</div>
        </div>
        
        <div class="text-center bg-white/70 p-4 rounded-xl">
          <div class="text-2xl font-bold text-purple-600">2 Anni</div>
          <div class="text-sm text-gray-600">Di Sviluppo</div>
        </div>
      </div>
    </div>
  </div>

  <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 mb-8">
    <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-green-600 to-blue-600 bg-clip-text text-transparent">
      Il percorso di sviluppo
    </h2>
    
    <div class="space-y-6">
      <div class="border-l-4 border-blue-500 pl-6">
        <h3 class="text-xl font-semibold text-gray-900 mb-2">Fase 1: Le Fondamenta (2023)</h3>
        <p class="text-gray-700 leading-relaxed">
          I primi mesi sono stati dedicati all'apprendimento del framework <strong>ESX</strong> e del linguaggio <strong>Lua</strong>. Partendo da zero, ho dovuto imparare non solo la sintassi, ma anche la logica che governa i server FiveM: dalla gestione dei giocatori alla creazione di lavori personalizzati.
        </p>
      </div>
      
      <div class="border-l-4 border-purple-500 pl-6">
        <h3 class="text-xl font-semibold text-gray-900 mb-2">Fase 2: Personalizzazione e Innovazione (2024)</h3>
        <p class="text-gray-700 leading-relaxed">
          Una volta acquisite le basi, il focus si è spostato sulla <strong>personalizzazione</strong>. Abbiamo sviluppato sistemi unici: un'economia dinamica che si adatta al comportamento dei giocatori, lavori innovativi che vanno oltre i classici "poliziotto e criminale", e un sistema di proprietà immobiliari complesso.
        </p>
      </div>
      
      <div class="border-l-4 border-green-500 pl-6">
        <h3 class="text-xl font-semibold text-gray-900 mb-2">Fase 3: Gestione della Comunità (2024-2025)</h3>
        <p class="text-gray-700 leading-relaxed">
          La crescita del progetto ha portato nuove sfide: gestire test collaborativi, moderare conflitti nel team, organizzare eventi di sviluppo e mantenere l'equilibrio delle meccaniche di gioco. Ho imparato che programmare è solo metà del lavoro - l'altra metà è coordinare le persone.
        </p>
      </div>
    </div>
  </div>

  <div class="bg-gradient-to-r from-red-50 to-orange-50 rounded-3xl p-8 mb-8 border-l-4 border-red-500">
    <h2 class="text-3xl font-bold mb-6 text-red-800">
      Le sfide tecniche superate
    </h2>
    
    <div class="grid md:grid-cols-2 gap-6">
      <div>
        <h3 class="text-lg font-semibold text-red-700 mb-3">Ottimizzazione delle Performance</h3>
        <p class="text-gray-700 text-sm leading-relaxed">
          Con l'espansione del progetto, il server iniziava a rallentare. Ho dovuto imparare a ottimizzare query SQL, ridurre i loop inutili in Lua e implementare sistemi di cache per migliorare le prestazioni.
        </p>
      </div>
      
      <div>
        <h3 class="text-lg font-semibold text-red-700 mb-3">Sicurezza e Anti-Cheat</h3>
        <p class="text-gray-700 text-sm leading-relaxed">
          Proteggere il server da exploit e cheater è stata una battaglia costante. Ho sviluppato sistemi di rilevamento automatico e implementato controlli server-side per ogni azione critica.
        </p>
      </div>
      
      <div>
        <h3 class="text-lg font-semibold text-red-700 mb-3">Backup e Disaster Recovery</h3>
        <p class="text-gray-700 text-sm leading-relaxed">
          Dopo aver perso dati una volta per un crash del database, ho implementato un sistema di backup automatico ogni 6 ore e procedure di ripristino rapido.
        </p>
      </div>
      
      <div>
        <h3 class="text-lg font-semibold text-red-700 mb-3">Interfacce Utente Responsive</h3>
        <p class="text-gray-700 text-sm leading-relaxed">
          Creare UI che funzionassero perfettamente in-game richiedeva competenze in HTML/CSS/JS e comprensione dell'integrazione con FiveM.
        </p>
      </div>
    </div>
  </div>

  <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8 mb-8">
    <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-orange-600 to-red-600 bg-clip-text text-transparent">
      Competenze acquisite
    </h2>
    
    <div class="grid md:grid-cols-3 gap-6">
      <div class="text-center p-6 bg-gradient-to-br from-blue-50 to-blue-100 rounded-2xl">
        <div class="text-4xl mb-4">💻</div>
        <h3 class="text-lg font-semibold text-blue-800 mb-2">Programmazione</h3>
        <ul class="text-sm text-gray-600 space-y-1">
          <li>• Lua scripting avanzato</li>
          <li>• SQL e ottimizzazione DB</li>
          <li>• HTML/CSS/JavaScript</li>
          <li>• Debugging e testing</li>
        </ul>
      </div>
      
      <div class="text-center p-6 bg-gradient-to-br from-green-50 to-green-100 rounded-2xl">
        <div class="text-4xl mb-4">🛠️</div>
        <h3 class="text-lg font-semibold text-green-800 mb-2">Gestione Sistema</h3>
        <ul class="text-sm text-gray-600 space-y-1">
          <li>• Amministrazione server Linux</li>
          <li>• Monitoraggio performance</li>
          <li>• Backup e sicurezza</li>
          <li>• Troubleshooting</li>
        </ul>
      </div>
      
      <div class="text-center p-6 bg-gradient-to-br from-purple-50 to-purple-100 rounded-2xl">
        <div class="text-4xl mb-4">👥</div>
        <h3 class="text-lg font-semibold text-purple-800 mb-2">Soft Skills</h3>
        <ul class="text-sm text-gray-600 space-y-1">
          <li>• Leadership di team</li>
          <li>• Gestione conflitti</li>
          <li>• Comunicazione efficace</li>
          <li>• Problem solving</li>
        </ul>
      </div>
    </div>
  </div>


  <div class="text-center">
    <button 
      onclick={() => navigateTo('capolavori')}
      class="bg-gradient-to-r from-purple-500 to-blue-600 text-white px-8 py-4 rounded-2xl font-semibold hover:shadow-2xl hover:shadow-purple-500/25 transition-all duration-300 transform hover:scale-105"
    >
      ← Torna ai Capolavori
    </button>
  </div>
</div>

<style>
  .animation-delay-1000 {
    animation-delay: 1s;
  }
</style>