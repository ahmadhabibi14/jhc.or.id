<script lang="ts">
  import Head from "@/partials/Head.svelte";
	import AboutUs from "@/partials/home/AboutUs.svelte";
	import Contact from "@/partials/home/Contact.svelte";
	import CorporateValue from "@/partials/home/CorporateValue.svelte";
	import Jumbotron from "@/partials/home/Jumbotron.svelte";
	import Services from "@/partials/home/Services.svelte";
	import StepHalal from "@/partials/home/StepHalal.svelte";
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
  <Services />
  <StepHalal />
  <Contact />
</div>