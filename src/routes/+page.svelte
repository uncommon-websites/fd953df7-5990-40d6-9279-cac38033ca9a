<script lang="ts">
  // Icons
  import { MessageSquare, Brain, Users, Zap, Shield, Globe, ArrowRight, Plus, Play, User, Quote, CheckCircle2 } from 'lucide-svelte';

  // State for FAQ
  let openFaq = -1;
  const faqs = [
    {
      q: "How does Delphi create a digital clone?",
      a: "Delphi uses your existing content—videos, podcasts, articles, and transcripts—to train a custom AI model that captures your unique knowledge, tone, and personality."
    },
    {
      q: "Is the clone's advice authentic?",
      a: "Yes. Unlike generic AI, your Delphi clone is strictly grounded in your provided content. It won't make things up or use external data unless you explicitly allow it."
    },
    {
      q: "Who owns the data and the clone?",
      a: "You do. You have full ownership of your data and your digital mind. You can update, pause, or delete your clone at any time."
    },
    {
      q: "How do coaches use Delphi?",
      a: "Coaches use Delphi to provide 24/7 support to their clients, answer common questions, and offer personalized mentorship at scale without being personally available at all hours."
    },
    {
      q: "Can I see real examples of conversations?",
      a: "Absolutely. We believe in transparency. You can view real, anonymized transcripts from existing clones to see how they handle complex, nuanced questions."
    }
  ];

  function toggleFaq(index: number) {
    openFaq = openFaq === index ? -1 : index;
  }
</script>

<main class="w-full overflow-hidden bg-white text-gray-900">
  <!-- Hero Section -->
  <section class="max-w-[1400px] mx-auto px-6 pt-20 pb-24">
    <div class="flex flex-col lg:flex-row justify-between items-start gap-12 mb-16">
      <div class="max-w-3xl">
        <h1 class="text-6xl md:text-[90px] leading-[0.9] font-medium tracking-tighter mb-10 text-black">
          Your mind.<br><span class="text-gray-400">Extended.</span>
        </h1>
        <div class="flex flex-wrap gap-4">
          <button class="bg-black text-white px-8 py-4 rounded-full font-medium hover:bg-gray-800 transition-all transform hover:scale-105 text-sm">
            Get early access
          </button>
          <button class="bg-white text-black border border-gray-200 px-8 py-4 rounded-full font-medium hover:bg-gray-50 transition-all text-sm">
            Talk to sales
          </button>
        </div>
      </div>
      
      <div class="max-w-sm pt-2 lg:pt-4">
        <p class="text-gray-500 text-lg leading-relaxed">
          Delphi creates interactive digital clones trained on your authentic content—so your expertise can speak for itself, even when you're not in the room.
        </p>
      </div>
    </div>

    <!-- Hero Image -->
    <div class="relative w-full aspect-[21/9] bg-gray-100 rounded-3xl overflow-hidden shadow-2xl border border-gray-100">
        <img src="/generated/image-a-high-end-minimalist-workspace-with-a-p-1768600507364-0.webp" alt="Delphi Digital Clone Interface" class="w-full h-full object-cover" />
        <div class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent"></div>
    </div>
  </section>

  <!-- Mission Section -->
  <section class="bg-black text-white py-32">
    <div class="max-w-[1000px] mx-auto px-6 text-center">
      <span class="text-sm font-medium text-gray-400 mb-6 block uppercase tracking-widest">Our Mission</span>
      <h2 class="text-4xl md:text-6xl font-medium tracking-tight mb-12 leading-tight">
        Democratizing wisdom by scaling human intelligence.
      </h2>
      <p class="text-gray-400 text-xl max-w-2xl mx-auto leading-relaxed mb-12">
        We believe everyone should have access to the world's best mentors. Delphi makes personalized mentorship accessible by allowing experts to be in 100,000 places at once.
      </p>
      <div class="flex justify-center gap-12">
          <div class="text-center">
              <div class="text-4xl font-bold mb-2">100K</div>
              <div class="text-gray-500 text-sm">Digital Minds</div>
          </div>
          <div class="text-center">
              <div class="text-4xl font-bold mb-2">$50B</div>
              <div class="text-gray-500 text-sm">Knowledge Economy</div>
          </div>
      </div>
    </div>
  </section>

  <!-- Features Grid -->
  <section class="max-w-[1400px] mx-auto px-6 py-32">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-24 items-center mb-32">
        <div>
            <h3 class="text-4xl font-medium mb-6 tracking-tight">Authenticity over automation</h3>
            <p class="text-gray-600 text-lg leading-relaxed mb-8">
                Rather than generic AI answers, Delphi lets your digital mind respond in your tone, your language, your way. All powered by your content, with full transparency and control.
            </p>
            <ul class="space-y-4">
                <li class="flex items-center gap-3 text-gray-700">
                    <CheckCircle2 class="text-black" size={20} />
                    <span>Trained exclusively on your content</span>
                </li>
                <li class="flex items-center gap-3 text-gray-700">
                    <CheckCircle2 class="text-black" size={20} />
                    <span>Captures your unique voice and nuance</span>
                </li>
                <li class="flex items-center gap-3 text-gray-700">
                    <CheckCircle2 class="text-black" size={20} />
                    <span>Real-time learning from new data</span>
                </li>
            </ul>
        </div>
        <div class="bg-gray-50 rounded-3xl p-8 border border-gray-100">
            <img src="/generated/image-close-up-of-a-tablet-showing-a-chat-inte-1768600614424-1.webp" alt="Authentic Conversation" class="rounded-2xl shadow-lg w-full" />
        </div>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-24 items-center">
        <div class="order-2 md:order-1 bg-gray-900 rounded-3xl p-12 text-white">
            <div class="mb-8">
                <Quote size={48} class="text-gray-700 mb-4" />
                <p class="text-2xl font-light italic leading-relaxed">
                    "I experienced crushing loneliness as a solo founder and created my grandfather's digital clone for guidance. That was the spark for Delphi."
                </p>
            </div>
            <div class="flex items-center gap-4">
                <img src="/generated/image-dara-ladjevardian-a-modern-tech-founder--1768600675272-2.webp" alt="Dara Ladjevardian" class="w-16 h-16 rounded-full object-cover border-2 border-gray-700" />
                <div>
                    <div class="font-bold">Dara Ladjevardian</div>
                    <div class="text-gray-400 text-sm">Co-Founder, Delphi</div>
                </div>
            </div>
        </div>
        <div class="order-1 md:order-2">
            <h3 class="text-4xl font-medium mb-6 tracking-tight">Proof in conversation</h3>
            <p class="text-gray-600 text-lg leading-relaxed mb-8">
                No hype—just transcripts. See how real users are building lasting communities and passive value through digital minds that actually sound like them.
            </p>
            <div class="space-y-4">
                <div class="p-4 bg-gray-50 rounded-xl border border-gray-100 flex items-start gap-4">
                    <div class="w-10 h-10 bg-black rounded-full flex items-center justify-center text-white shrink-0">
                        <MessageSquare size={18} />
                    </div>
                    <div>
                        <div class="text-sm font-bold mb-1">User Question</div>
                        <div class="text-sm text-gray-600">"How do I handle burnout when scaling my business?"</div>
                    </div>
                </div>
                <div class="p-4 bg-white rounded-xl border border-gray-200 shadow-sm flex items-start gap-4 ml-8">
                    <div class="w-10 h-10 bg-gray-200 rounded-full flex items-center justify-center shrink-0 overflow-hidden">
                        <img src="/generated/image-sam-spelsberg-a-technical-tech-founder-w-1768600750347-3.webp" alt="Clone" class="w-full h-full object-cover" />
                    </div>
                    <div>
                        <div class="text-sm font-bold mb-1">Expert Clone</div>
                        <div class="text-sm text-gray-800">"Burnout isn't about the work, it's about the lack of recovery. In my 2021 workshop, I talked about the 'Sprint-Rest' cycle..."</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </section>

  <!-- Founders Section -->
  <section class="bg-gray-50 py-32">
    <div class="max-w-[1400px] mx-auto px-6">
        <div class="text-center mb-20">
            <h2 class="text-4xl font-medium tracking-tight mb-4">Built by founders who needed mentorship</h2>
            <p class="text-gray-600 max-w-2xl mx-auto">Dara and Sam co-founded Delphi to scale human intelligence and make personalized mentorship accessible to everyone.</p>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-12 max-w-4xl mx-auto">
            <div class="bg-white p-8 rounded-3xl border border-gray-100 shadow-sm">
                <img src="/generated/image-dara-ladjevardian-a-modern-tech-founder--1768600675272-2.webp" alt="Dara Ladjevardian" class="w-full aspect-square rounded-2xl object-cover mb-6" />
                <h3 class="text-xl font-bold mb-2">Dara Ladjevardian</h3>
                <p class="text-sm text-gray-500 mb-4 uppercase tracking-wider">Co-Founder</p>
                <p class="text-gray-600 text-sm leading-relaxed">
                    Dara's first-generation immigrant background and personal need for mentorship drive his mission to democratize wisdom access.
                </p>
            </div>
            <div class="bg-white p-8 rounded-3xl border border-gray-100 shadow-sm">
                <img src="/generated/image-sam-spelsberg-a-technical-tech-founder-w-1768600750347-3.webp" alt="Sam Spelsberg" class="w-full aspect-square rounded-2xl object-cover mb-6" />
                <h3 class="text-xl font-bold mb-2">Sam Spelsberg</h3>
                <p class="text-sm text-gray-500 mb-4 uppercase tracking-wider">Co-Founder</p>
                <p class="text-gray-600 text-sm leading-relaxed">
                    Sam's technical expertise and vision for conversational media position him to transform how knowledge transfers between minds.
                </p>
            </div>
        </div>
    </div>
  </section>

  <!-- FAQ Section -->
  <section class="max-w-[800px] mx-auto px-6 py-32">
      <h2 class="text-3xl font-medium mb-12 text-center">Frequently asked questions</h2>
      
      <div class="divide-y divide-gray-100 border-y border-gray-100">
          {#each faqs as faq, i}
            <div class="py-6">
                <button class="w-full flex items-center justify-between text-left group" on:click={() => toggleFaq(i)}>
                    <span class="text-lg font-medium text-gray-900 group-hover:text-black transition-colors">{faq.q}</span>
                    <span class="text-gray-400">
                        <Plus size={20} class="transition-transform duration-200 {openFaq === i ? 'rotate-45' : ''}" />
                    </span>
                </button>
                {#if openFaq === i}
                    <div class="mt-4 text-gray-600 leading-relaxed pb-2">
                        {faq.a}
                    </div>
                {/if}
            </div>
          {/each}
      </div>
  </section>

  <!-- Bottom CTA -->
  <section class="max-w-[1400px] mx-auto px-6 py-32 flex flex-col items-center text-center">
      <div class="bg-black text-white w-full rounded-[40px] py-24 px-6 overflow-hidden relative">
          <!-- Decorative background elements -->
          <div class="absolute top-0 right-0 w-96 h-96 bg-gray-800 rounded-full blur-[120px] -mr-48 -mt-48 opacity-50"></div>
          <div class="absolute bottom-0 left-0 w-96 h-96 bg-gray-800 rounded-full blur-[120px] -ml-48 -mb-48 opacity-50"></div>
          
          <h2 class="text-5xl md:text-7xl font-medium tracking-tight mb-8 relative z-10">You’re not replaceable.<br>But you are replicable.</h2>
          <p class="text-gray-400 text-xl mb-12 max-w-2xl mx-auto relative z-10">
              Make your knowledge accessible—without losing what makes it yours. Join the waitlist for Delphi today.
          </p>
          <div class="flex flex-col sm:flex-row items-center justify-center gap-4 relative z-10">
              <button class="bg-white text-black px-10 py-5 rounded-full font-bold hover:bg-gray-100 transition-all transform hover:scale-105">
                  Get Early Access
              </button>
              <button class="bg-transparent text-white border border-white/20 px-10 py-5 rounded-full font-bold hover:bg-white/10 transition-all">
                  View Demo
              </button>
          </div>
      </div>
  </section>
</main>

<style>
    :global(html) {
        scroll-behavior: smooth;
    }
</style>

