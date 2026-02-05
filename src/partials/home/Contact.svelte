<script lang="ts">
  function getAcademicYear(): number {
    const now = new Date();
    const month = now.getMonth(); // 0 = Jan, 10 = Nov, 11 = Dec
    const year = now.getFullYear();

    return month >= 10 ? year + 1 : year;
  }

  const year: number = getAcademicYear();
  const contacts: {
    title: string;
    link: string;
    img: string;
    content: string;
  }[] = [
    {
      title: "Location",
      link: "https://maps.app.goo.gl/D5JcyKYwyHBXSkWc6",
      img: "/icons/contact/location.svg",
      content: "Jl. Assyafi'iyah No.247, RT.3/RW.5, Cilangkap, Kec. Cipayung, Jakarta Timur, DKI Jakarta. 13870"
    },
    {
      title: "Email",
      link: "mailto:jayakartahalalcenter@gmail.com",
      img: "/icons/contact/mail.svg",
      content: "jayakartahalalcenter@gmail.com"
    },
    {
      title: "WhatsApp",
      link: "https://wa.me/6282146021999",
      img: "/icons/contact/whatsapp.svg",
      content: "(+62) 813-2248-2220"
    }
  ]
</script>

<section class="w-full h-auto bg-jhc-2 text-white py-28 relative overflow-hidden md:px-0 px-5" id="kontak">
  <div class="absolute w-full h-full mx-auto flex justify-center items-center -top-10">
    <img
      src="/icons/mosaic-jhc-2.svg"
      alt="Mosaic Light"
      class="w-150 h-auto"
    />
  </div>
  <div class="container max-w-6xl mx-auto flex flex-col gap-6 justify-center items-center relative z-10">
    <h3 class="text-5xl text-center leading-14 font-bold">Siap Menuju <span class="text-jhc-orange">Sertifikasi</span> <br/> <span class="text-jhc-orange">Halal {year}?</span></h3>
    <p class="font-light text-lg md:w-9/12 text-center">Amankan izin edar dan kepatuhan halal produk Anda sebelum batas wajib 2026. Tim ahli kami siap mendampingi Anda sekarang</p>
    <div class="flex flex-col md:gap-1 gap-3 md:w-6/12 mx-auto px-auto py-6 text-sm md:text-base">
      {#each contacts as con}
        <a
          href={con.link}
          target="_blank"
          class="flex flex-row gap-2 items-center hover:underline hover:text-jhc-light md:h-12 h-auto"
        >
          <img
            src={con.img}
            alt={con.title}
            class="h-10 w-auto"
          />
          <p class="grow">{con.content}</p>
        </a>
      {/each}
    </div>
    <div class="flex md:flex-row flex-col justify-center items-center gap-4 font-medium">
      <a href="https://wa.me/6281322482220" target="_blank" class="bg-jhc-orange text-jhc py-3 px-7 rounded-full cursor-pointer hover:bg-jhc-orange/90 shadow-2xl border border-jhc-orange">
        Daftar Sertifikasi Sekarang
      </a>
      <a href="https://wa.me/6281322482220" target="_blank" class="text-white py-3 px-7 rounded-full cursor-pointer shadow-2xl border border-white hover:bg-white/10">
        Konsultasi Gratis
      </a>
    </div>
  </div>
</section>