<script lang="ts">
  const services: {
    title: string;
    desc: string;
    img: string;
  }[] = [
    {
      title: 'Konsultasi',
      desc: 'JHC Memposisikan diri sebagai mitra strategis yang memberikan solusi halal komprehensif, mulai dari pemetaan kebutuhan, pemenuhan regulasi, hingga perbaikan berkelanjutan sesuai standar halal nasional.',
      img: '/icons/services/konsultasi.svg'
    },
    {
      title: 'Edukasi',
      desc: 'JHC Memposisikan diri sebagai mitra strategis yang memberikan solusi halal komprehensif, mulai dari pemetaan kebutuhan, pemenuhan regulasi, hingga perbaikan berkelanjutan sesuai standar halal nasional.',
      img: '/icons/services/edukasi.svg'
    },
    {
      title: 'Training',
      desc: 'JHC Memposisikan diri sebagai mitra strategis yang memberikan solusi halal komprehensif, mulai dari pemetaan kebutuhan, pemenuhan regulasi, hingga perbaikan berkelanjutan sesuai standar halal nasional.',
      img: '/icons/services/training.svg'
    },
    {
      title: 'Sertifikasi',
      desc: 'JHC Memposisikan diri sebagai mitra strategis yang memberikan solusi halal komprehensif, mulai dari pemetaan kebutuhan, pemenuhan regulasi, hingga perbaikan berkelanjutan sesuai standar halal nasional.',
      img: '/icons/services/sertifikasi.svg'
    }
  ]
</script>

<section class="container max-w-6xl mx-auto mb-16 mt-10 md:px-0 px-5" id="layanan">
  <div class="flex flex-col gap-7">
    <div class="flex flex-col gap-2 text-center">
      <span class="text-jhc-orange text-xl font-medium">Layanan Kami</span>
      <h3 class="text-jhc font-semibold text-4xl">Positioning Jayakarta Halal Center</h3>
    </div>

    <div class="md:grid md:grid-cols-2 md:grid-rows-2 flex flex-col gap-5">
      {#each services as s}
        <div class="flex flex-row items-start gap-4 shadow-md border border-gray-200 p-6 rounded-xl">
          <img
            src={s.img}
            alt={s.title}
            class="md:w-20 w-15 h-auto shrink-0"
          />
          <div class="grow flex flex-col gap-1">
            <h4 class="text-2xl font-semibold">{s.title}</h4>
            <p class="text-sm">{s.desc}</p>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>