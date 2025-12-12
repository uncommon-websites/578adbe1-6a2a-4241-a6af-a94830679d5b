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
      <h2 class="text-sm font-semibold mb-6 text-primary-600 tracking-wide">The Future of Sharehouse Living</h2>
      
      <h1 class="text-5xl md:text-7xl font-bold tracking-tight leading-[1.1] mb-10">
        <div class="flex flex-wrap justify-center items-center gap-x-3 gap-y-2">
          <span>Live together</span>
        </div>
        <div class="flex flex-wrap justify-center items-center gap-x-3 gap-y-2">
          <span>without the</span>
          <span class="inline-flex items-center justify-center w-12 h-12 md:w-16 md:h-16 bg-gradient-to-br from-gray-50 to-gray-100 rounded-2xl align-middle mx-1">
            <DollarIcon className="w-6 h-6 md:w-8 md:h-8" />
          </span>
          <span>stress</span>
        </div>
      </h1>

      <p class="text-lg md:text-xl text-gray-600 mb-10 max-w-2xl leading-relaxed">
        Imagine a sharehouse where bills split themselves, reminders happen automatically, and everyone knows exactly what they owe. No arguments. No confusion. Just harmony.
      </p>

      <div class="mb-12">
        <Button>
          <Apple className="w-5 h-5" />
          <span class="text-base">Download for iOS</span>
        </Button>
      </div>

      <!-- Social Proof -->
      <div class="flex flex-wrap justify-center gap-16 text-gray-400 text-xs font-medium">
        <div class="flex flex-col items-center leading-tight">
          <span class="text-3xl font-bold text-black mb-2">2M+</span>
          <span class="text-gray-500 text-sm">Sharehouses in Australia</span>
        </div>
        <div class="flex flex-col items-center leading-tight">
          <span class="text-3xl font-bold text-black mb-2">Zero</span>
          <span class="text-gray-500 text-sm">Arguments about money</span>
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
      <div class="rounded-3xl overflow-hidden">
        <img 
          src="/generated/image-young-housemates-laughing-together-in-a--1765501958639-0.webp" 
          alt="Happy housemates enjoying stress-free living together"
          class="w-full h-auto"
        />
      </div>
      <div class="text-center mt-8 max-w-2xl mx-auto">
        <p class="text-lg text-gray-600 leading-relaxed italic">
          This is what sharehouse life looks like when the admin takes care of itself
        </p>
      </div>
    </section>

    <!-- How It Works Section -->
    <section class="w-full bg-gradient-to-b from-gray-50 to-white py-24 mb-32">
      <div class="max-w-3xl mx-auto px-6 text-center">
        <h2 class="text-sm font-semibold mb-6 text-primary-600 uppercase tracking-wide">How It Works</h2>
        <h3 class="text-3xl md:text-5xl font-bold tracking-tight leading-tight mb-6">
          Three steps to complete peace of mind
        </h3>
        <p class="text-lg text-gray-600 mb-16 max-w-2xl mx-auto">
          Set it up once, then forget about the admin. Homerun runs in the background so you can focus on actually living together.
        </p>
        
        <div class="grid md:grid-cols-3 gap-12 text-left">
          <div class="space-y-4">
            <div class="w-14 h-14 bg-gradient-to-br from-black to-gray-800 text-white rounded-2xl flex items-center justify-center font-bold text-xl mb-4">1</div>
            <h4 class="text-xl font-bold">Upload Your Lease</h4>
            <p class="text-gray-600 leading-relaxed">Drop in your lease PDF and watch as every detail extracts itself. No typing, no manual entry, no hassle.</p>
          </div>
          
          <div class="space-y-4">
            <div class="w-14 h-14 bg-gradient-to-br from-black to-gray-800 text-white rounded-2xl flex items-center justify-center font-bold text-xl mb-4">2</div>
            <h4 class="text-xl font-bold">Invite Housemates</h4>
            <p class="text-gray-600 leading-relaxed">One link brings everyone into the same dashboard. Instant transparency, zero confusion about who owes what.</p>
          </div>
          
          <div class="space-y-4">
            <div class="w-14 h-14 bg-gradient-to-br from-black to-gray-800 text-white rounded-2xl flex items-center justify-center font-bold text-xl mb-4">3</div>
            <h4 class="text-xl font-bold">Live Stress-Free</h4>
            <p class="text-gray-600 leading-relaxed">Bills split automatically. Reminders arrive on time. Everyone knows their share. You get back to enjoying life together.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Features Text -->
    <section class="max-w-5xl mx-auto px-6 pb-32 space-y-32 text-center">
      <!-- Feature 1: Peace of Mind -->
      <div class="space-y-8">
        <div class="inline-flex items-center justify-center w-20 h-20 bg-gradient-to-br from-gray-100 to-gray-50 rounded-3xl mb-4">
          <DocumentIcon className="w-10 h-10" />
        </div>
        <h3 class="text-4xl md:text-6xl font-bold tracking-tight leading-tight max-w-3xl mx-auto">
          Never think about lease details again
        </h3>
        <p class="text-xl text-gray-600 max-w-2xl mx-auto leading-relaxed">
          Upload once and forget. Your rent schedule, bond amount, and key dates live in one place where everyone can see them. No more digging through emails or asking "when's rent due?"
        </p>
      </div>

      <!-- Lifestyle Image: Cooking Together -->
      <div class="w-full max-w-5xl mx-auto">
        <div class="rounded-3xl overflow-hidden">
          <img 
            src="/generated/image-group-of-diverse-young-adults-cooking-to-1765501926455-1.webp" 
            alt="Housemates cooking together in harmony"
            class="w-full h-auto"
          />
        </div>
        <p class="text-center text-gray-500 mt-6 text-sm italic">
          When the money stuff is handled, you can focus on what actually matters
        </p>
      </div>

      <!-- Feature 2: Financial Harmony -->
      <div class="space-y-8">
        <div class="inline-flex items-center justify-center w-20 h-20 bg-gradient-to-br from-gray-100 to-gray-50 rounded-3xl mb-4">
          <DollarIcon className="w-10 h-10" />
        </div>
        <h3 class="text-4xl md:text-6xl font-bold tracking-tight leading-tight max-w-3xl mx-auto">
          Money conversations without the awkwardness
        </h3>
        <p class="text-xl text-gray-600 max-w-2xl mx-auto leading-relaxed">
          Everyone sees exactly what they owe, when it's due, and who's paid. No more chasing people down or feeling uncomfortable asking for money. Just complete transparency and fairness.
        </p>
      </div>

      <!-- Feature 3: Time Freedom -->
      <div class="space-y-8">
        <div class="inline-flex items-center justify-center w-20 h-20 bg-gradient-to-br from-gray-100 to-gray-50 rounded-3xl mb-4">
          <PeopleIcon className="w-10 h-10" />
        </div>
        <h3 class="text-4xl md:text-6xl font-bold tracking-tight leading-tight max-w-3xl mx-auto">
          Get your evenings and weekends back
        </h3>
        <p class="text-xl text-gray-600 max-w-2xl mx-auto leading-relaxed">
          No more spreadsheet updates, group chat marathons, or Sunday afternoon admin sessions. Homerun handles it all in the background so you can actually enjoy living together.
        </p>
      </div>

      <!-- Lifestyle Image: Relaxing -->
      <div class="w-full max-w-3xl mx-auto">
        <div class="rounded-3xl overflow-hidden">
          <img 
            src="/generated/image-young-professional-relaxing-on-a-couch-w-1765501928950-2.webp" 
            alt="Relaxed housemate enjoying stress-free living"
            class="w-full h-auto"
          />
        </div>
        <p class="text-center text-gray-500 mt-6 text-sm italic">
          This is what stress-free sharehouse living feels like
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
      <div class="space-y-10">
        <h2 class="text-4xl md:text-6xl font-bold tracking-tight leading-tight">
          Start living stress-free today
        </h2>
        <p class="text-xl text-gray-600 max-w-2xl mx-auto leading-relaxed">
          Imagine coming home to a house where the bills are handled, everyone knows what they owe, and money never creates tension. That's not a dream. That's what happens when you use Homerun.
        </p>
        <div class="pt-6">
          <Button>
            <Apple className="w-5 h-5" />
            <span class="text-base">Download for iOS</span>
          </Button>
        </div>
        <p class="text-sm text-gray-500">Free forever. Set up in under 5 minutes.</p>
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


