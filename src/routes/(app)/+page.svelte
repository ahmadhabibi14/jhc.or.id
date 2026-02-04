<script lang="ts">
  import Head from "@/partials/Head.svelte";
	import AboutUs from "@/partials/home/AboutUs.svelte";
	import Contact from "@/partials/home/Contact.svelte";
	import Jumbotron from "@/partials/home/Jumbotron.svelte";
	import VisiMisi from "@/partials/home/VisiMisi.svelte";
</script>

<Head
  title="Jasa Sertifikasi Halal Resmi & Terpercaya - Jayakarta Halal Center"
/>

<div class="min-h-[900px] w-full flex flex-col gap-7 md:gap-10">
  <Jumbotron />
  <AboutUs />
  <VisiMisi />
  <Contact />
</div>