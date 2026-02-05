<script lang="ts">
	import { Icon } from "svelte-icons-pack";
	import { RiCommunicationChatSmile2Fill } from "svelte-icons-pack/ri";
</script>

<section class="container max-w-6xl mx-auto" id="tentang">
  <div class="flex flex-col gap-5">
    <div class="text-sm bg-jhc-light border border-jhc text-jhc font-medium flex flex-row items-center gap-2 w-fit rounded-full py-1.5 px-4">
      <Icon
        src={RiCommunicationChatSmile2Fill}
        size={20}
        className="fill-jhc text-jhc"
      />
      <span>Tentang Kami</span>
    </div>
    <div class="grid grid-cols-2 gap-10">
      <div class="flex flex-col gap-6">
        <h2 class="text-4xl font-bold text-jhc">Mitra Strategis <br /> Legalisasi Halal Anda</h2>
        <div class="flex flex-col gap-4">
          <p>JAYAKARTA HALAL CENTER (JHC) merupakan lembaga konsultan halal yang
  berfokus pada pendampingan, edukasi, dan penguatan ekosistem halal di
  Indonesia. Jayakarta Halal Center (JHC) siap membantu para Pelaku Usaha dalam
  mendapatkan sertifikat halal pada produk usaha makanan, kosmetik,
  produk kimiawi, produk rekayasa genetik dan barang gunaan
  serta usaha jasa.
  </p>
  <p>
  JHC memastikan kehalalan produk dan proses produk halal para
  Pelaku Usaha dapat terjamin dengan proses yang komprehensif melalui
  pemeriksaan oleh Lembaga Pemeriksa Halal (LPH) terpercaya untuk
  memastikan kualitas, keamanan, dan kepatuhan produk terhadap
  standar halal yang telah ditetapkan.</p>
        </div>
      </div>
      <div class="shadow-md rounded-xl p-5 grid grid-cols-2 grid-rows-2 w-full h-80 gap-5 border border-gray-100">
        <div class="flex flex-col gap-3 justify-center items-center w-full h-auto border border-jhc-2 rounded-xl bg-jhc-light/50 text-jhc-2">
          <span class="font-bold text-3xl">100+</span>
          <span>DAPUR BERSERTIFIKAT</span>
        </div>
        <div class="flex flex-col gap-3 justify-center items-center w-full h-auto border border-gray-300 rounded-xl bg-white">
          <span class="font-bold text-3xl text-jhc-orange">99%</span>
          <span>TINGKAT KELULUSAN</span>
        </div>
        <div class="flex flex-col gap-3 justify-center items-center w-full h-auto border border-purple-400 rounded-xl bg-purple-400/20 text-purple-600">
          <span class="font-bold text-3xl">0</span>
          <span>REVISI MAYOR</span>
        </div>
        <div class="flex flex-col gap-3 justify-center items-center w-full h-auto border border-gray-400 rounded-xl bg-gray-400/20 text-gray-600">
          <span class="font-bold text-3xl">24/7</span>
          <span>SUPPORT TIM</span>
        </div>
      </div>
    </div>
  </div>
</section>