<script>
  let { currentPage, navigateTo } = $props();

  const navItems = [
    { id: 'home', label: 'Home', icon: '🏠' },
    { id: 'blog', label: 'Blog', icon: '📝' },
    { id: 'pcto', label: 'PCTO', icon: '💼' },
    { id: 'capolavori', label: 'Capolavori', icon: '🎨' },
    { id: 'chi-sono', label: 'Chi Sono', icon: '👤' }
  ];
</script>

<nav class="bg-white/90 backdrop-blur-md shadow-lg border-b border-white/20 sticky top-0 z-50">
  <div class="container mx-auto px-4">
    <div class="flex items-center justify-between h-16">
      <div class="flex items-center space-x-3 group">
        <div class="text-3xl transform group-hover:scale-110 transition-transform duration-300">🎓</div>
        <div>
          <h1 class="text-xl font-bold bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
            Educazione Civica
          </h1>
          <p class="text-xs text-gray-500">Portfolio Digitale</p>
        </div>
      </div>
      
      <div class="hidden md:flex space-x-2">
        {#each navItems as item}
          <button
            onclick={() => navigateTo(item.id)}
            class="flex items-center space-x-2 px-4 py-2 rounded-xl text-sm font-medium transition-all duration-300 transform hover:scale-105
                   {currentPage === item.id 
                     ? 'bg-gradient-to-r from-blue-500 to-purple-500 text-white shadow-lg shadow-blue-500/25' 
                     : 'text-gray-600 hover:text-gray-900 hover:bg-white/80 hover:shadow-md'}"
          >
            <span class="text-lg">{item.icon}</span>
            <span>{item.label}</span>
          </button>
        {/each}
      </div>

      <!-- Mobile menu button con animazione -->
      <div class="md:hidden">
        <button class="text-gray-600 hover:text-gray-900 p-2 rounded-lg hover:bg-white/50 transition-all duration-300" aria-label="Open Menu">
          <svg class="h-6 w-6 transform hover:rotate-90 transition-transform duration-300" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>
    </div>

    <!-- Mobile menu migliorato -->
    <div class="md:hidden border-t border-white/20 bg-white/95 backdrop-blur-sm">
      <div class="px-2 pt-2 pb-3 space-y-1">
        {#each navItems as item}
          <button
            onclick={() => navigateTo(item.id)}
            class="flex items-center space-x-3 w-full px-4 py-3 rounded-xl text-base font-medium transition-all duration-300
                   {currentPage === item.id 
                     ? 'bg-gradient-to-r from-blue-500 to-purple-500 text-white shadow-lg' 
                     : 'text-gray-600 hover:text-gray-900 hover:bg-white/80'}"
          >
            <span class="text-xl">{item.icon}</span>
            <span>{item.label}</span>
          </button>
        {/each}
      </div>
    </div>
  </div>
</nav>
