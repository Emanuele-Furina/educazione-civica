<script>
  import { onMount } from 'svelte';
  import Navigation from './lib/components/Navigation.svelte';
  import Home from './lib/pages/Home.svelte';
  import Blog from './lib/pages/Blog.svelte';
  import PCTO from './lib/pages/PCTO.svelte';
  import Capolavori from './lib/pages/Capolavori.svelte';
  import ChiSono from './lib/pages/ChiSono.svelte';
  import PenaDiMorte from './lib/articles/PenaDiMorte.svelte';
  import StoriaMafia from './lib/articles/StoriaMafia.svelte';
  import ViolenzaGenere from './lib/articles/ViolenzaGenere.svelte';
  import WarPoetry from './lib/articles/WarPoetry.svelte';
  import CarcareSperanza from './lib/articles/CarcareSperanza.svelte';

  let currentPage = $state('home');

  function navigateTo(page) {
    currentPage = page;
    // Update URL without page reload for GitHub Pages compatibility
    window.history.pushState({}, '', `#${page}`);
  }

  onMount(() => {
    // Handle initial page load and browser back/forward
    const handleHashChange = () => {
      const hash = window.location.hash.slice(1);
      const validPages = ['home', 'blog', 'pcto', 'capolavori', 'chi-sono'];
      const validArticles = ['pena-di-morte', 'storia-mafia', 'violenza-genere', 'war-poetry', 'carcere-speranza'];
    
      if (hash && (validPages.includes(hash) || validArticles.includes(hash))) {
        currentPage = hash;
      }
    };

    handleHashChange();
    window.addEventListener('hashchange', handleHashChange);

    return () => {
      window.removeEventListener('hashchange', handleHashChange);
    };
  });
</script>

<div class="min-h-screen bg-gradient-to-br from-blue-50 via-indigo-50 to-purple-50">
  <Navigation {currentPage} {navigateTo} />
  
  <main class="container mx-auto px-4 py-8">
    <div class="animate-fade-in">
      {#if currentPage === 'home'}
        <Home />
      {:else if currentPage === 'blog'}
        <Blog {navigateTo} />
      {:else if currentPage === 'pcto'}
        <PCTO />
      {:else if currentPage === 'capolavori'}
        <Capolavori />
      {:else if currentPage === 'chi-sono'}
        <ChiSono />
      {:else if currentPage === 'pena-di-morte'}
        <PenaDiMorte {navigateTo} />
      {:else if currentPage === 'storia-mafia'}
        <StoriaMafia {navigateTo} />
      {:else if currentPage === 'violenza-genere'}
        <ViolenzaGenere {navigateTo} />
      {:else if currentPage === 'war-poetry'}
        <WarPoetry {navigateTo} />
      {:else if currentPage === 'carcere-speranza'}
        <CarcareSperanza {navigateTo} />
      {/if}
    </div>
  </main>

  <footer class="bg-white/80 backdrop-blur-sm border-t border-white/20 mt-16">
    <div class="container mx-auto px-4 py-8 text-center text-gray-600">
      <div class="flex items-center justify-center space-x-2 mb-4">
        <span class="text-2xl">🎓</span>
        <span class="font-semibold">Educazione Civica Portfolio</span>
      </div>
      <p>&copy; 2024 Emanuele Furina - Realizzato con ❤️ e Svelte</p>
    </div>
  </footer>
</div>

<style>
  @keyframes fade-in {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  
  .animate-fade-in {
    animation: fade-in 0.6s ease-out;
  }
</style>
