<script lang="ts">
  import Header from '$lib/components/Header.svelte';
  import Button from '$lib/components/Button.svelte';
  import Apple from '$lib/components/icons/Apple.svelte';
  import HouseIcon from '$lib/components/icons/HouseIcon.svelte';
  import DollarIcon from '$lib/components/icons/DollarIcon.svelte';
  import PeopleIcon from '$lib/components/icons/PeopleIcon.svelte';
  import DocumentIcon from '$lib/components/icons/DocumentIcon.svelte';
  import Laurel from '$lib/components/icons/Laurel.svelte';
  import PhoneUI from '$lib/components/PhoneUI.svelte';
</script>

<svelte:head>
  <title>Homerun - Sharehouse Admin & Bill Splitting Made Simple</title>
  <meta name="description" content="Upload your lease, invite your housemates, and let Homerun handle the rest. Fair splits, automated reminders, and zero arguments. Built for Australian sharehouses." />
  <meta property="og:title" content="Homerun - Sharehouse Admin & Bill Splitting Made Simple" />
  <meta property="og:description" content="Upload your lease, invite your housemates, and let Homerun handle the rest. Fair splits, automated reminders, and zero arguments." />
  <meta property="og:type" content="website" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Homerun - Sharehouse Admin & Bill Splitting Made Simple" />
  <meta name="twitter:description" content="Upload your lease, invite your housemates, and let Homerun handle the rest. Fair splits, automated reminders, and zero arguments." />
</svelte:head>

<div class="min-h-screen bg-white text-black font-sans selection:bg-gray-200">
  <Header />

  <main class="flex flex-col items-center w-full">
    <!-- Hero Section -->
    <section class="flex flex-col items-center text-center pt-10 pb-12 px-4 max-w-4xl mx-auto">
      <h2 class="text-sm font-semibold mb-6 text-primary-600">Sharehouse Admin, Simplified</h2>
      
      <h1 class="text-5xl md:text-7xl font-bold tracking-tight leading-[1.1] mb-10">
        <div class="flex flex-wrap justify-center items-center gap-x-3 gap-y-2">
          <span>Run your</span>
          <span class="inline-flex items-center justify-center w-12 h-12 md:w-16 md:h-16 bg-gray-100 rounded-2xl align-middle mx-1">
            <HouseIcon className="w-6 h-6 md:w-8 md:h-8" />
          </span>
          <span>sharehouse</span>
        </div>
        <div class="flex flex-wrap justify-center items-center gap-x-3 gap-y-2">
          <span>without the</span>
          <span class="inline-flex items-center justify-center w-12 h-12 md:w-16 md:h-16 bg-gray-100 rounded-2xl align-middle mx-1">
            <DollarIcon className="w-6 h-6 md:w-8 md:h-8" />
          </span>
          <span>chaos</span>
        </div>
      </h1>

      <p class="text-lg md:text-xl text-gray-600 mb-10 max-w-2xl">
        Upload your lease, invite your housemates, and let Homerun handle the rest. Fair splits, automated reminders, and zero arguments.
      </p>

      <div class="mb-12">
        <Button>
          <Apple className="w-5 h-5" />
          <span class="text-base">Download for iOS</span>
        </Button>
      </div>

      <!-- Social Proof -->
      <div class="flex flex-wrap justify-center gap-8 text-gray-400 text-xs font-medium">
        <div class="flex flex-col items-center leading-tight">
          <span class="text-2xl font-bold text-black mb-1">2M+</span>
          <span class="text-gray-500">Australian Sharehouses</span>
        </div>
        <div class="flex flex-col items-center leading-tight">
          <span class="text-2xl font-bold text-black mb-1">$8B</span>
          <span class="text-gray-500">Rental Admin Market</span>
        </div>
      </div>
    </section>

    <!-- Phone Showcase -->
    <section class="w-full max-w-[1000px] px-4 mb-24 relative flex justify-center">
      <!-- Background glow/shadow simulation -->
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[600px] h-[600px] bg-gray-100/50 rounded-full blur-3xl -z-10"></div>
      
      <!-- Phone Container -->
      <div class="relative w-[300px] md:w-[340px] h-[680px] md:h-[720px] transition-transform hover:scale-[1.02] duration-500">
        <PhoneUI />
      </div>
    </section>

    <!-- Lifestyle Image Section -->
    <section class="w-full max-w-5xl mx-auto px-6 mb-32">
      <div class="rounded-3xl overflow-hidden shadow-2xl">
        <img 
          src="/generated/image-young-australian-housemates-sitting-toge-1765496313691-0.webp" 
          alt="Young housemates collaborating on household admin"
          class="w-full h-auto"
        />
      </div>
    </section>

    <!-- How It Works Section -->
    <section class="w-full bg-gray-50 py-24 mb-32">
      <div class="max-w-3xl mx-auto px-6 text-center">
        <h2 class="text-sm font-semibold mb-6 text-primary-600 uppercase tracking-wide">How It Works</h2>
        <h3 class="text-3xl md:text-5xl font-bold tracking-tight leading-tight mb-12">
          Three steps to stress-free sharehouse living
        </h3>
        
        <div class="grid md:grid-cols-3 gap-8 text-left">
          <div class="space-y-3">
            <div class="w-12 h-12 bg-black text-white rounded-2xl flex items-center justify-center font-bold text-xl mb-4">1</div>
            <h4 class="text-xl font-bold">Upload Your Lease</h4>
            <p class="text-gray-600">Drop in your lease PDF and we'll extract all the important details automatically.</p>
          </div>
          
          <div class="space-y-3">
            <div class="w-12 h-12 bg-black text-white rounded-2xl flex items-center justify-center font-bold text-xl mb-4">2</div>
            <h4 class="text-xl font-bold">Invite Housemates</h4>
            <p class="text-gray-600">Send a link to your housemates and they're instantly added to your shared dashboard.</p>
          </div>
          
          <div class="space-y-3">
            <div class="w-12 h-12 bg-black text-white rounded-2xl flex items-center justify-center font-bold text-xl mb-4">3</div>
            <h4 class="text-xl font-bold">Let Homerun Handle It</h4>
            <p class="text-gray-600">Automated reminders, fair splits, and bill comparisons keep everything running smoothly.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Features Text -->
    <section class="max-w-4xl mx-auto px-6 pb-32 space-y-24 text-center">
      <div class="space-y-6">
        <div class="inline-flex items-center justify-center w-16 h-16 bg-gradient-to-br from-gray-100 to-gray-50 rounded-2xl mb-4 shadow-sm">
          <DocumentIcon className="w-8 h-8" />
        </div>
        <h3 class="text-3xl md:text-5xl font-bold tracking-tight leading-tight">
          Upload your lease and we'll extract everything automatically
        </h3>
        <p class="text-lg text-gray-600 max-w-2xl mx-auto">
          No more manual data entry. Homerun reads your lease PDF and sets up rent schedules, bond amounts, key dates, and house structure in seconds.
        </p>
      </div>

      <div class="space-y-6">
        <div class="inline-flex items-center justify-center w-16 h-16 bg-gradient-to-br from-gray-100 to-gray-50 rounded-2xl mb-4 shadow-sm">
          <DollarIcon className="w-8 h-8" />
        </div>
        <h3 class="text-3xl md:text-5xl font-bold tracking-tight leading-tight">
          Split bills fairly and save money on every expense
        </h3>
        <p class="text-lg text-gray-600 max-w-2xl mx-auto">
          Compare electricity, gas, and internet offers in your area. Track shared expenses automatically. Get discounts on household essentials through our subscription box.
        </p>
      </div>

      <div class="space-y-10">
        <div class="inline-flex items-center justify-center w-16 h-16 bg-gradient-to-br from-gray-100 to-gray-50 rounded-2xl mb-4 shadow-sm">
          <PeopleIcon className="w-8 h-8" />
        </div>
        <h3 class="text-3xl md:text-5xl font-bold tracking-tight leading-tight">
          Built for renters, by someone who lived the chaos
        </h3>
        <p class="text-lg text-gray-600 max-w-2xl mx-auto">
          Scott created Homerun after years of sharehouse frustration in Sydney. No more group chat confusion, missed payments, or unfair splits. Just a simple dashboard that works.
        </p>
      </div>
    </section>

    <!-- Founder Story Section -->
    <section class="w-full max-w-4xl mx-auto px-6 pb-32">
      <div class="bg-gray-50 rounded-3xl p-8 md:p-12">
        <div class="max-w-2xl mx-auto text-center space-y-6">
          <div class="text-4xl mb-4">"</div>
          <p class="text-xl md:text-2xl font-medium leading-relaxed">
            I lived in a 5-person sharehouse in Surry Hills for years. The constant confusion about who owed what, missed bill payments, and group chat chaos drove me crazy. I built Homerun to fix the problems I experienced every single day.
          </p>
          <div class="pt-4">
            <div class="font-bold text-lg">Scott</div>
            <div class="text-gray-600">Founder, Homerun</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Final CTA Section -->
    <section class="w-full max-w-4xl mx-auto px-6 pb-32 text-center">
      <div class="space-y-8">
        <h2 class="text-4xl md:text-6xl font-bold tracking-tight leading-tight">
          Ready to simplify your sharehouse?
        </h2>
        <p class="text-xl text-gray-600 max-w-2xl mx-auto">
          Join thousands of Australian renters who've ditched the spreadsheets and group chat chaos.
        </p>
        <div class="pt-4">
          <Button>
            <Apple className="w-5 h-5" />
            <span class="text-base">Download for iOS</span>
          </Button>
        </div>
        <p class="text-sm text-gray-500">Free to use. No credit card required.</p>
      </div>
    </section>

    <!-- Footer -->
    <footer class="w-full py-12 flex flex-col items-center gap-6 text-center border-t border-gray-100 mt-auto">
      <div class="font-bold text-xl tracking-tight text-gray-200">Homerun</div>
      <div class="flex flex-wrap justify-center gap-4 text-xs text-gray-400 font-medium">
        <a href="#" class="hover:text-black transition-colors">App Store</a>
        <span>•</span>
        <a href="#" class="hover:text-black transition-colors">Contact</a>
        <span>•</span>
        <a href="#" class="hover:text-black transition-colors">X (FKA Twitter)</a>
        <span>•</span>
        <a href="#" class="hover:text-black transition-colors">Privacy policy</a>
      </div>
      <div class="text-[10px] text-gray-300">
        Built in Sydney for Australian renters
      </div>
    </footer>
  </main>
</div>


