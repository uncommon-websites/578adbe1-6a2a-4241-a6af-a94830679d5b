<script lang="ts">
  import Header from '$lib/components/Header.svelte';
  import Button from '$lib/components/Button.svelte';
  import Apple from '$lib/components/icons/Apple.svelte';
  import DollarIcon from '$lib/components/icons/DollarIcon.svelte';
  import DocumentIcon from '$lib/components/icons/DocumentIcon.svelte';
  import LightningIcon from '$lib/components/icons/LightningIcon.svelte';
  import PhoneUI from '$lib/components/PhoneUI.svelte';
</script>

<svelte:head>
  <title>Homerun — Sharehouse admin, sorted</title>
  <meta name="description" content="Upload your lease, invite your housemates, and let Homerun handle the rest. Automatic bill splitting, shared dashboards, and zero awkward money conversations." />
  <meta property="og:title" content="Homerun — Sharehouse admin, sorted" />
  <meta property="og:description" content="Upload your lease, invite your housemates, and let Homerun handle the rest. Automatic bill splitting, shared dashboards, and zero awkward money conversations." />
  <meta property="og:type" content="website" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Homerun — Sharehouse admin, sorted" />
  <meta name="twitter:description" content="Upload your lease, invite your housemates, and let Homerun handle the rest. Automatic bill splitting, shared dashboards, and zero awkward money conversations." />
</svelte:head>

<style>
  @keyframes fadeUp {
    from {
      opacity: 0;
      transform: translateY(24px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
  }

  @keyframes scaleIn {
    from {
      opacity: 0;
      transform: scale(0.96);
    }
    to {
      opacity: 1;
      transform: scale(1);
    }
  }

  .animate-fade-up {
    animation: fadeUp 0.6s cubic-bezier(0.16, 1, 0.3, 1) both;
  }

  .animate-fade-in {
    animation: fadeIn 0.8s ease-out both;
  }

  .animate-scale-in {
    animation: scaleIn 0.7s cubic-bezier(0.16, 1, 0.3, 1) both;
  }

  .delay-100 { animation-delay: 100ms; }
  .delay-200 { animation-delay: 200ms; }
  .delay-300 { animation-delay: 300ms; }
  .delay-400 { animation-delay: 400ms; }
  .delay-500 { animation-delay: 500ms; }
  .delay-600 { animation-delay: 600ms; }

  @media (prefers-reduced-motion: reduce) {
    .animate-fade-up,
    .animate-fade-in,
    .animate-scale-in {
      animation: none;
    }
  }
</style>

<div class="min-h-screen bg-white text-black font-sans selection:bg-gray-200">
  <Header />

  <main class="flex flex-col items-center w-full">

    <!-- Hero Section -->
    <section class="flex flex-col items-center text-center pt-16 pb-16 px-6 max-w-5xl mx-auto w-full">
      
      <!-- Badge -->
      <div class="animate-fade-up inline-flex items-center gap-2 bg-gray-50 border border-gray-200 rounded-full px-4 py-1.5 mb-10">
        <span class="w-1.5 h-1.5 rounded-full bg-green-500 inline-block"></span>
        <span class="text-xs font-semibold text-gray-600 tracking-wide">Free for Australian sharehouses</span>
      </div>

      <h1 class="animate-fade-up delay-100 text-5xl md:text-7xl font-bold tracking-tight leading-[1.08] mb-8 text-balance">
        Sharehouse admin,<br />
        <span class="text-gray-400">finally sorted</span>
      </h1>

      <p class="animate-fade-up delay-200 text-lg md:text-xl text-gray-500 mb-10 max-w-xl leading-relaxed text-pretty">
        Upload your lease, invite your housemates, and let Homerun handle the rest. Bills split automatically. Everyone knows what they owe. No more group chat chaos.
      </p>

      <div class="animate-fade-up delay-300 flex flex-col sm:flex-row items-center gap-4 mb-16">
        <Button>
          <Apple className="w-5 h-5" />
          <span>Download for iOS</span>
        </Button>
        <span class="text-sm text-gray-400 font-medium">Free forever · 5 min setup</span>
      </div>

      <!-- Stats row -->
      <div class="animate-fade-up delay-400 flex flex-wrap justify-center gap-12 md:gap-20">
        <div class="text-center">
          <div class="text-3xl font-bold tracking-tight mb-1">2M+</div>
          <div class="text-sm text-gray-500">Sharehouses in Australia</div>
        </div>
        <div class="w-px bg-gray-100 hidden md:block self-stretch"></div>
        <div class="text-center">
          <div class="text-3xl font-bold tracking-tight mb-1">$0</div>
          <div class="text-sm text-gray-500">Cost to use Homerun</div>
        </div>
        <div class="w-px bg-gray-100 hidden md:block self-stretch"></div>
        <div class="text-center">
          <div class="text-3xl font-bold tracking-tight mb-1">Zero</div>
          <div class="text-sm text-gray-500">Awkward money chats</div>
        </div>
      </div>
    </section>

    <!-- Phone Showcase -->
    <section class="w-full max-w-[1100px] px-6 mb-28 relative flex justify-center">
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[500px] h-[500px] bg-gray-100/60 rounded-full blur-3xl -z-10 pointer-events-none"></div>
      <div class="animate-scale-in delay-200 relative w-[290px] md:w-[330px] h-[640px] md:h-[700px] transition-transform hover:scale-[1.02] duration-700 ease-out">
        <PhoneUI />
      </div>
    </section>

    <!-- Lifestyle Hero Image -->
    <section class="w-full max-w-6xl mx-auto px-6 mb-32">
      <div class="animate-scale-in rounded-[2rem] overflow-hidden ring-1 ring-gray-100 hover:ring-gray-200 transition-all duration-500">
        <img 
          src="/generated/image-young-housemates-laughing-together-in-a--1765501958639-0.webp" 
          alt="Happy housemates enjoying stress-free living together"
          class="w-full h-auto block"
          loading="lazy"
        />
      </div>
      <p class="text-center mt-8 text-gray-400 text-sm font-medium">
        This is what sharehouse life looks like when the admin takes care of itself
      </p>
    </section>

    <!-- How It Works -->
    <section class="relative w-full py-28 mb-28 overflow-hidden">
      <div class="absolute inset-0 bg-gray-50/70 -z-10"></div>
      <div class="absolute top-0 right-0 w-[500px] h-[500px] bg-gradient-to-bl from-primary-50/40 to-transparent rounded-full blur-3xl -z-10 pointer-events-none"></div>
      
      <div class="max-w-5xl mx-auto px-6 text-center">
        <p class="text-xs font-bold text-primary-600 tracking-[0.2em] uppercase mb-6">How it works</p>
        <h2 class="text-4xl md:text-5xl font-bold tracking-tight leading-tight mb-6 text-balance">
          Three steps to peace of mind
        </h2>
        <p class="text-lg text-gray-500 mb-20 max-w-2xl mx-auto leading-relaxed">
          Set it up once, then forget about the admin. Homerun runs quietly in the background while you focus on actually living together.
        </p>
        
        <div class="grid md:grid-cols-3 gap-12 text-left">
          <div class="group">
            <div class="w-14 h-14 bg-black text-white rounded-2xl flex items-center justify-center font-bold text-xl mb-6 group-hover:scale-110 group-hover:-rotate-2 transition-all duration-300 ease-out">1</div>
            <h3 class="text-xl font-bold mb-3">Upload your lease</h3>
            <p class="text-gray-500 leading-relaxed">Drop in your lease PDF and Homerun extracts every detail automatically. Rent schedule, bond amount, key dates — all done.</p>
          </div>
          
          <div class="group">
            <div class="w-14 h-14 bg-black text-white rounded-2xl flex items-center justify-center font-bold text-xl mb-6 group-hover:scale-110 group-hover:-rotate-2 transition-all duration-300 ease-out">2</div>
            <h3 class="text-xl font-bold mb-3">Invite your housemates</h3>
            <p class="text-gray-500 leading-relaxed">One link brings everyone onto the same dashboard. Instant transparency, zero confusion about who owes what and when.</p>
          </div>
          
          <div class="group">
            <div class="w-14 h-14 bg-black text-white rounded-2xl flex items-center justify-center font-bold text-xl mb-6 group-hover:scale-110 group-hover:-rotate-2 transition-all duration-300 ease-out">3</div>
            <h3 class="text-xl font-bold mb-3">Live stress-free</h3>
            <p class="text-gray-500 leading-relaxed">Bills split automatically. Reminders go out on time. Everyone knows their share. You get back to enjoying life together.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Feature Sections -->
    <section class="w-full max-w-5xl mx-auto px-6 pb-28">

      <!-- Feature 1 -->
      <div class="grid md:grid-cols-2 gap-16 items-center mb-32">
        <div class="space-y-6">
          <div class="inline-flex items-center justify-center w-14 h-14 bg-gray-50 border border-gray-100 rounded-2xl">
            <DocumentIcon className="w-7 h-7 text-gray-700" />
          </div>
          <h2 class="text-3xl md:text-4xl font-bold tracking-tight leading-tight text-balance">
            Your lease, decoded in seconds
          </h2>
          <p class="text-gray-500 leading-relaxed text-lg">
            Upload your PDF and Homerun reads it for you. Rent schedules, bond amounts, inspection dates — extracted automatically and shared with everyone in the house. No more "when's rent due?" in the group chat.
          </p>
        </div>
        <div class="rounded-2xl overflow-hidden bg-gray-50 ring-1 ring-gray-100">
          <img 
            src="/generated/image-group-of-diverse-young-adults-cooking-to-1765501926455-1.webp" 
            alt="Housemates relaxed and organised"
            class="w-full h-auto block"
            loading="lazy"
          />
        </div>
      </div>

      <!-- Feature 2 -->
      <div class="grid md:grid-cols-2 gap-16 items-center mb-32">
        <div class="order-2 md:order-1 rounded-2xl overflow-hidden bg-gray-50 ring-1 ring-gray-100">
          <img 
            src="/generated/image-group-of-housemates-having-coffee-on-a-s-1765501965968-2.webp" 
            alt="Housemates enjoying time together without money stress"
            class="w-full h-auto block"
            loading="lazy"
          />
        </div>
        <div class="order-1 md:order-2 space-y-6">
          <div class="inline-flex items-center justify-center w-14 h-14 bg-gray-50 border border-gray-100 rounded-2xl">
            <DollarIcon className="w-7 h-7 text-gray-700" />
          </div>
          <h2 class="text-3xl md:text-4xl font-bold tracking-tight leading-tight text-balance">
            Fair splits, without the friction
          </h2>
          <p class="text-gray-500 leading-relaxed text-lg">
            Everyone sees exactly what they owe, when it's due, and who's already paid. No more chasing people down or feeling awkward about asking for money. Just complete transparency, every time.
          </p>
        </div>
      </div>

      <!-- Feature 3 -->
      <div class="grid md:grid-cols-2 gap-16 items-center">
        <div class="space-y-6">
          <div class="inline-flex items-center justify-center w-14 h-14 bg-gray-50 border border-gray-100 rounded-2xl">
            <LightningIcon className="w-7 h-7 text-gray-700" />
          </div>
          <h2 class="text-3xl md:text-4xl font-bold tracking-tight leading-tight text-balance">
            Save money on top of saving time
          </h2>
          <p class="text-gray-500 leading-relaxed text-lg">
            Compare electricity, gas, and internet deals in your area. Get discounts on household essentials. Homerun doesn't just organise your home — it helps you afford it.
          </p>
        </div>
        <div class="rounded-2xl overflow-hidden bg-gray-50 ring-1 ring-gray-100">
          <img 
            src="/generated/image-young-professional-relaxing-on-a-couch-w-1765501928950-2.webp" 
            alt="Young renter relaxing stress-free at home"
            class="w-full h-auto block"
            loading="lazy"
          />
        </div>
      </div>
    </section>

    <!-- Founder Story -->
    <section class="w-full max-w-4xl mx-auto px-6 pb-32">
      <div class="bg-gray-50 rounded-3xl p-10 md:p-16 border border-gray-100">
        <div class="max-w-2xl mx-auto text-center space-y-6">
          <svg class="w-8 h-8 text-gray-300 mx-auto" viewBox="0 0 32 32" fill="currentColor">
            <path d="M9.352 4C4.456 7.456 1 13.12 1 19.36c0 5.088 3.072 8.064 6.624 8.064 3.36 0 5.856-2.688 5.856-5.856 0-3.168-2.208-5.472-5.088-5.472-.576 0-1.344.096-1.536.192.48-3.264 3.552-7.104 6.624-9.024L9.352 4zm16.512 0c-4.8 3.456-8.256 9.12-8.256 15.36 0 5.088 3.072 8.064 6.624 8.064 3.264 0 5.856-2.688 5.856-5.856 0-3.168-2.304-5.472-5.184-5.472-.576 0-1.248.096-1.44.192.48-3.264 3.456-7.104 6.528-9.024L25.864 4z"/>
          </svg>
          <p class="text-xl md:text-2xl font-medium leading-relaxed text-gray-800">
            I lived in a 5-person sharehouse in Surry Hills for years. The constant confusion about who owed what, missed bill payments, and group chat chaos drove me crazy. I built Homerun to fix the problems I experienced every single day.
          </p>
          <div class="pt-2">
            <div class="font-bold text-base">Scott</div>
            <div class="text-gray-500 text-sm">Founder, Homerun · Sydney, Australia</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Final CTA -->
    <section class="relative w-full max-w-4xl mx-auto px-6 pb-40 text-center">
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[500px] h-[300px] bg-gradient-to-br from-gray-100/60 to-transparent rounded-full blur-3xl -z-10 pointer-events-none"></div>
      
      <div class="space-y-8">
        <h2 class="text-5xl md:text-6xl font-bold tracking-tight leading-[1.08] text-balance">
          Your sharehouse,<br />
          <span class="text-gray-400">running itself</span>
        </h2>
        <p class="text-xl text-gray-500 max-w-xl mx-auto leading-relaxed">
          Join thousands of Australian renters who've traded group chat chaos for a home that actually runs smoothly.
        </p>
        <div class="pt-4">
          <Button>
            <Apple className="w-5 h-5" />
            <span>Download for iOS</span>
          </Button>
        </div>
        <p class="text-sm text-gray-400">Free forever · Set up in under 5 minutes</p>
      </div>
    </section>

    <!-- Footer -->
    <footer class="w-full py-12 border-t border-gray-100">
      <div class="max-w-5xl mx-auto px-6 flex flex-col md:flex-row items-center justify-between gap-6">
        <div class="font-bold text-lg tracking-tight text-gray-900">Homerun</div>
        <div class="flex flex-wrap justify-center gap-6 text-sm text-gray-400">
          <a href="#" class="hover:text-black transition-colors duration-200">App Store</a>
          <a href="#" class="hover:text-black transition-colors duration-200">Contact</a>
          <a href="#" class="hover:text-black transition-colors duration-200">Twitter</a>
          <a href="#" class="hover:text-black transition-colors duration-200">Privacy policy</a>
        </div>
        <div class="text-xs text-gray-300">Built in Sydney for Australian renters</div>
      </div>
    </footer>

  </main>
</div>


