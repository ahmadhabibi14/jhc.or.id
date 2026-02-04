<script lang="ts">
	import { Icon } from "svelte-icons-pack";
	import { RiSystemCheckboxCircleFill } from "svelte-icons-pack/ri";

</script>
<div role="banner" id="jumbotron">
  <div class="w-full min-h-[500px] z-1 bg-jhc-light flex">
    <div class="container max-w-6xl mx-auto">
      <div class="grid grid-cols-[60%_1fr] gap-10 items-center h-full">
        <div class="flex flex-col gap-4">
          <div class="w-fit h-fit py-1 px-3 text-jhc flex flex-row gap-2 items-center justify-center bg-white rounded-full">
            <Icon
              src={RiSystemCheckboxCircleFill}
              size="16"
              className="text-jhc fill-jhc"
            />
            <span>Jasa Sertifikasi Halal Terpercaya</span>
          </div>
          <h1 class="text-6xl font-bold text-jhc leading-16">Sertifikasi Halal <br /> <span class="text-jhc-orange">Presisi & Terarah</span></h1>
          <p>Kami memimpin pendampingan dan pengurusan sertifikasi halal bagi UMKM, Pabrik, Hingga Instansi Nasional</p>
          <div class="flex flex-row gap-4">
            <button class="py-2 px-6 rounded-full bg-jhc hover:bg-jhc-2 text-white cursor-pointer border border-jhc">
              Daftar Sekarang
            </button>
            <button class="py-2 px-6 rounded-full bg-white hover:bg-gray-100 cursor-pointer border border-jhc">
              Digitalisasi Dokumen
            </button>
          </div>
        </div>
        <div class="w-96 h-auto">
          <img
            src="/img/hero.png"
            alt="Hero"
            class="w-auto h-auto"
          />
        </div>
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
</div>