<script lang="ts">
  function getAcademicYear(): number {
    const now = new Date();
    const month = now.getMonth(); // 0 = Jan, 10 = Nov, 11 = Dec
    const year = now.getFullYear();

    return month >= 10 ? year + 1 : year;
  }

  const year = getAcademicYear();
</script>

<section class="w-full h-auto bg-jhc-2 text-white py-28" id="kontak">
  <div class="container max-w-6xl mx-auto flex flex-col gap-6 justify-center items-center">
    <h3 class="text-5xl text-center leading-14 font-bold">Siap Menuju <span class="text-jhc-orange">Sertifikasi</span> <br/> <span class="text-jhc-orange">Halal {year}?</span></h3>
    <p class="font-light text-lg w-9/12 text-center">Amankan izin edar dan kepatuhan halal produk Anda sebelum batas wajib 2026. Tim ahli kami siap mendampingi Anda sekarang</p>
    <div class="flex flex-row gap-4 font-medium mt-9">
      <a href="https://wa.me/6281322482220" target="_blank" class="bg-jhc-orange text-jhc py-3 px-7 rounded-full cursor-pointer hover:bg-jhc-orange/90 shadow-2xl border border-jhc-orange">
        Daftar Sertifikasi Sekarang
      </a>
      <a href="https://wa.me/6281322482220" target="_blank" class="text-white py-3 px-7 rounded-full cursor-pointer shadow-2xl border border-white hover:bg-white/10">
        Konsultasi Gratis
      </a>
    </div>
  </div>
</section>