<script lang="ts">
	import { Icon } from "svelte-icons-pack";
	import { RiSystemCheckboxCircleFill } from "svelte-icons-pack/ri";
</script>

<section role="banner" id="jumbotron">
  <div class="w-full z-1 bg-jhc-light flex">
    <div class="container max-w-6xl mx-auto pt-10 md:pt-20 pb-6 md:pb-0">
      <div class="flex flex-col-reverse md:grid md:grid-cols-[1fr_auto] gap-10 items-center h-full px-6 md:px-0">
        <div class="flex flex-col gap-4 relative">
          <img
            src="/icons/duo-quotes.svg"
            alt="Quotes"
            class="absolute -left-[10%] top-13 lg:w-10 h-auto lg:block hidden"
          />
          <div class="w-fit h-fit py-1 px-3 text-jhc flex flex-row gap-2 items-center justify-center bg-white rounded-full">
            <Icon
              src={RiSystemCheckboxCircleFill}
              size="18"
              className="text-jhc fill-jhc"
            />
            <span>Jasa Sertifikasi Halal Terpercaya</span>
          </div>
          <h1 class="text-3xl md:text-5xl font-bold text-jhc md:leading-12">Solusi Halal Brand <br /> <span class="text-jhc-orange">Handal, Cepat, Legal</span></h1>
          <p class="md:w-10/12 w-full">Kami memimpin pendampingan dan pengurusan sertifikasi halal bagi UMKM, Pabrik, Hingga Instansi Nasional</p>
          <div class="flex flex-col md:flex-row gap-4">
            <a href="https://wa.me/6281322482220" target="_blank" class="w-fit py-2 px-6 rounded-full bg-jhc hover:bg-jhc-2 text-white cursor-pointer border border-jhc">
              Daftar Sekarang
            </a>
            <a href="https://wa.me/6281322482220" target="_blank" class="w-fit py-2 px-6 rounded-full bg-white hover:bg-gray-100 cursor-pointer border border-jhc">
              Digitalisasi Dokumen
            </a>
          </div>
        </div>
        <img
          src="/img/cert-pak-ade.png"
          alt="Hero"
          class="w-full md:w-auto h-auto md:h-100"
          fetchpriority="high"
        />
      </div>
    </div>
  </div>
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 200" class="text-jhc-light">
    <path
      fill="currentColor"
      fill-opacity="1"
      d="M0,96L60,106.7C120,117,240,139,360,128C480,117,600,75,720,80C840,85,960,139,1080,149.3C1200,160,1320,128,1380,112L1440,96L1440,0L1380,0C1320,0,1200,0,1080,0C960,0,840,0,720,0C600,0,480,0,360,0C240,0,120,0,60,0L0,0Z"
    >
    </path>
  </svg>
</section>