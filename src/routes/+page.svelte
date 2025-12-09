<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import Logos from "$lib/components/Logos.svelte";
  import ValueProp from "$lib/components/ValueProp.svelte";
  import Features from "$lib/components/Features.svelte";
  import Contexts from "$lib/components/Contexts.svelte";
  import Vision from "$lib/components/Vision.svelte";
  import Security from "$lib/components/Security.svelte";
  import Testimonial from "$lib/components/Testimonial.svelte";
  import CTA from "$lib/components/CTA.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<div class="min-h-screen bg-white font-sans text-black selection:bg-black selection:text-white">
  <Header />
  <main>
    <Hero />
    <Logos />
    <ValueProp />
    <Features />
    <Contexts />
    <Vision />
    <Security />
    <Testimonial />
    <CTA />
  </main>
  <Footer />
</div>

