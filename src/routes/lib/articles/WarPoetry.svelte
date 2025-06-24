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
      Back to Blog
    </button>

    <div class="text-center">
      <div class="flex items-center justify-center space-x-4 mb-6">
        <span class="bg-gradient-to-r from-indigo-500 to-purple-500 text-white text-sm font-bold px-4 py-2 rounded-full">Literature</span>
        <span class="text-gray-500">May 27, 2025</span>
        <span class="text-gray-500">8 min read</span>
      </div>
      
      <h1 class="text-4xl md:text-5xl font-bold mb-6 bg-gradient-to-r from-indigo-600 to-purple-600 bg-clip-text text-transparent leading-tight">
        War Poetry - Voices from the Battlefield
      </h1>
      
      <p class="text-xl text-gray-600 leading-relaxed max-w-3xl mx-auto">
        An analysis of war poetry through the lens of Rupert Brooke's "The Soldier", Wilfred Owen's "Dulce et Decorum Est", and W.H. Auden's "Refugee Blues" - exploring how literature captures the human cost of conflict.
      </p>
    </div>
  </header>

  <!-- Contenuto dell'articolo -->
  <div class="prose prose-lg max-w-none space-y-8">
    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-indigo-600 to-purple-600 bg-clip-text text-transparent">
        The Evolution of War Literature
      </h2>
      
      <p class="text-gray-700 leading-relaxed">
        War poetry has served as one of the most powerful means of documenting human conflict, evolving from glorified nationalism to stark realism and humanitarian concern. Through the works of poets like Rupert Brooke, Wilfred Owen, and W.H. Auden, we witness a transformation in how literature approaches war—from romantic idealization to brutal truth-telling and compassionate witness to suffering.
      </p>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-green-600 to-blue-600 bg-clip-text text-transparent">
        Rupert Brooke's "The Soldier" - Romantic Nationalism
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Rupert Brooke's "The Soldier" (1915) represents the early idealistic response to World War I, written before the full horror of trench warfare became apparent:
      </p>
      
      <blockquote class="border-l-4 border-green-500 pl-6 italic text-lg text-gray-700 mb-6 bg-green-50 p-4 rounded-r-lg">
        <em>"If I should die, think only this of me:<br>
        That there's some corner of a foreign field<br>
        That is for ever England."</em>
      </blockquote>

      <h3 class="text-2xl font-semibold mb-4 text-gray-800">Analysis</h3>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Brooke's poem embodies the <strong>romantic nationalism</strong> that characterized early war poetry. The speaker presents death in battle as a noble sacrifice, transforming foreign soil into sacred English ground. The poem's structure mirrors its content—orderly, traditional, reflecting the established values it celebrates.
      </p>
      
      <div class="bg-green-50 rounded-2xl p-6">
        <h4 class="font-semibold mb-3 text-green-800">Key themes:</h4>
        <ul class="space-y-2 text-gray-700">
          <li><strong>Patriotic sacrifice:</strong> Death becomes a gift to the homeland</li>
          <li><strong>Immortality through service:</strong> The soldier lives on in the land he dies for</li>
          <li><strong>Idealized England:</strong> The motherland as pure, nurturing force</li>
          <li><strong>Religious undertones:</strong> Battle death as blessed, almost Christ-like sacrifice</li>
        </ul>
      </div>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-red-600 to-orange-600 bg-clip-text text-transparent">
        Wilfred Owen's "Dulce et Decorum Est" - The Reality of War
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Written in 1917, Owen's "Dulce et Decorum Est" directly challenges Brooke's romanticized vision:
      </p>
      
      <blockquote class="border-l-4 border-red-500 pl-6 italic text-lg text-gray-700 mb-6 bg-red-50 p-4 rounded-r-lg">
        <em>"If you could hear, at every jolt, the blood<br>
        Come gargling from the froth-corrupted lungs,<br>
        Obscene as cancer, bitter as the cud<br>
        Of vile, incurable sores on innocent tongues,—<br>
        My friend, you would not tell with such high zest<br>
        To children ardent for some desperate glory,<br>
        The old Lie: Dulce et decorum est<br>
        Pro patria mori."</em>
      </blockquote>

      <h3 class="text-2xl font-semibold mb-4 text-gray-800">Analysis</h3>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Owen's poem represents a <strong>radical departure</strong> from traditional war poetry. Having experienced the trenches firsthand, Owen exposes the "old Lie" that it is sweet and proper to die for one's country.
      </p>
      
      <div class="grid md:grid-cols-2 gap-6">
        <div class="bg-red-50 rounded-2xl p-6">
          <h4 class="font-semibold mb-3 text-red-800">Structural elements:</h4>
          <ul class="space-y-2 text-gray-700">
            <li><strong>Irregular rhythm:</strong> Mimics chaos of battle</li>
            <li><strong>Vivid imagery:</strong> Gas attacks, drowning metaphors</li>
            <li><strong>Direct address:</strong> "My friend" makes reader complicit</li>
            <li><strong>Latin conclusion:</strong> Ironically quotes Horace</li>
          </ul>
        </div>
        
        <div class="bg-orange-50 rounded-2xl p-6">
          <h4 class="font-semibold mb-3 text-orange-800">Key themes:</h4>
          <ul class="space-y-2 text-gray-700">
            <li><strong>Anti-war message:</strong> War as dehumanizing horror</li>
            <li><strong>Betrayal of youth:</strong> Older generations sending young to die</li>
            <li><strong>Physical reality:</strong> Graphic descriptions counter abstractions</li>
            <li><strong>Moral responsibility:</strong> Writers must tell truth</li>
          </ul>
        </div>
      </div>
    </div>

    <div class="bg-white/70 backdrop-blur-sm rounded-3xl shadow-xl border border-white/20 p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
        W.H. Auden's "Refugee Blues" - War's Civilian Victims
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        Auden's "Refugee Blues" (1939) shifts focus from soldiers to civilians, addressing the plight of Jewish refugees fleeing Nazi persecution:
      </p>
      
      <blockquote class="border-l-4 border-blue-500 pl-6 italic text-lg text-gray-700 mb-6 bg-blue-50 p-4 rounded-r-lg">
        <em>"Say this city has ten million souls,<br>
        Some are living in mansions, some are living in holes:<br>
        Yet there's no place for us, my dear, yet there's no place for us."</em>
      </blockquote>

      <h3 class="text-2xl font-semibold mb-4 text-gray-800">Historical Context</h3>
      
      <p class="text-gray-700 leading-relaxed">
        The poems reflect their <strong>historical moments</strong>: 1915's early war optimism, 1917's trench warfare reality, and 1939's rising awareness of Nazi persecution and refugee crisis.
      </p>
    </div>

    <div class="bg-gradient-to-r from-indigo-50 to-purple-50 rounded-3xl p-8">
      <h2 class="text-3xl font-bold mb-6 bg-gradient-to-r from-indigo-600 to-purple-600 bg-clip-text text-transparent">
        The Enduring Power of War Poetry
      </h2>
      
      <p class="text-gray-700 leading-relaxed mb-6">
        These three poems demonstrate poetry's unique ability to capture war's <strong>human dimension</strong>. While history records dates and casualties, poetry preserves the <strong>emotional truth</strong> of conflict—the hope, horror, and suffering that statistics cannot convey.
      </p>
      
      <div class="bg-white/50 rounded-2xl p-6">
        <h3 class="text-xl font-semibold mb-4 text-gray-800">War poetry serves several crucial functions:</h3>
        <ul class="space-y-3 text-gray-700">
          <li><strong>Historical witness:</strong> Documenting experiences that might otherwise be forgotten</li>
          <li><strong>Moral testimony:</strong> Challenging comfortable assumptions about war and heroism</li>
          <li><strong>Emotional catharsis:</strong> Providing outlet for trauma and grief</li>
          <li><strong>Educational tool:</strong> Teaching empathy across time and cultural boundaries</li>
        </ul>
      </div>
      
      <blockquote class="border-l-4 border-indigo-500 pl-6 italic text-lg text-gray-700 mt-8">
        "My subject is War, and the pity of War. The Poetry is in the pity." – Wilfred Owen
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
        Back to Blog
      </button>
      
      <div class="flex space-x-4">
        <button class="bg-blue-100 text-blue-800 px-4 py-2 rounded-lg hover:bg-blue-200 transition-colors duration-300">
          Share
        </button>
        <button class="bg-gray-100 text-gray-800 px-4 py-2 rounded-lg hover:bg-gray-200 transition-colors duration-300">
          Print
        </button>
      </div>
    </div>
  </footer>
</article>
