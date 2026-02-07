<script lang="ts">
  import Head from "@/partials/Head.svelte";
	import AboutUs from "@/partials/home/AboutUs.svelte";
	import Benefit from "@/partials/home/Benefit.svelte";
	import Contact from "@/partials/home/Contact.svelte";
	import CorporateValue from "@/partials/home/CorporateValue.svelte";
	import IndustryUsage from "@/partials/home/IndustryUsage.svelte";
	import Jumbotron from "@/partials/home/Jumbotron.svelte";
	import Partners from "@/partials/home/Partners.svelte";
	import Services from "@/partials/home/Services.svelte";
	import StepHalal from "@/partials/home/StepHalal.svelte";
	import Testimonials from "@/partials/home/Testimonials.svelte";
	import TrustedBy from "@/partials/home/TrustedBy.svelte";
	import VisiMisi from "@/partials/home/VisiMisi.svelte";
</script>

<Head
  title="Jasa Sertifikasi Halal Resmi & Terpercaya - Jayakarta Halal Center"
/>

<div class="min-h-[900px] w-full flex flex-col">
  <Jumbotron />
  <AboutUs />
  <VisiMisi />
  <CorporateValue />
  <TrustedBy />
  <IndustryUsage />
  <Services />
  <StepHalal />
  <Benefit />
  <Testimonials />
  <Partners />
  <Contact />
</div>