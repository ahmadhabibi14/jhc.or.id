<script lang="ts">
  const testimonials: {
  content: string;
  name: string;
  role: string;
}[] = [
  {
    content:
      "Proses sertifikasi halal berjalan sangat jelas dan terarah. Timnya responsif, membantu dari tahap awal hingga sertifikat diterbitkan tanpa ribet.",
    name: "Ahmad Fauzi",
    role: "Owner UMKM Kuliner"
  },
  {
    content:
      "Pendampingan yang diberikan sangat profesional. Kami jadi lebih paham standar halal dan implementasinya di proses produksi.",
    name: "Siti Aisyah",
    role: "Quality Assurance Manager"
  },
  {
    content:
      "Layanannya cepat dan transparan. Setiap tahapan dijelaskan dengan bahasa yang mudah dipahami, sangat membantu bagi pelaku usaha.",
    name: "Rizky Pratama",
    role: "Founder Startup F&B"
  },
  {
    content:
      "Kami merasa terbantu dengan adanya konsultasi halal yang komprehensif, terutama dalam menyiapkan dokumen dan audit internal.",
    name: "Nurhaliza Putri",
    role: "Head of Operations"
  },
  {
    content:
      "Tim konsultan sangat komunikatif dan solutif. Sertifikasi halal yang awalnya terasa rumit jadi jauh lebih mudah.",
    name: "Muhammad Iqbal",
    role: "Direktur Produksi"
  },
  {
    content:
      "Pelayanan yang diberikan sesuai standar dan tepat waktu. Sangat cocok untuk perusahaan yang ingin memastikan kepatuhan halal secara menyeluruh.",
    name: "Dewi Lestari",
    role: "Compliance Officer"
  },
  {
    content:
      "Pendampingan dilakukan secara detail dan berkelanjutan. Tidak hanya sertifikasi, tapi juga edukasi halal bagi tim kami.",
    name: "Hendra Wijaya",
    role: "Manajer Pabrik"
  },
  {
    content:
      "Pengalaman kami sangat positif. Prosesnya efisien, komunikasinya jelas, dan hasilnya sesuai harapan.",
    name: "Fitri Ramadhani",
    role: "Pemilik Usaha Makanan Olahan"
  }
];
</script>

<section class="container max-w-6xl mx-auto my-16 md:px-5 lg:px-0 px-5" id="testimonials">
  <div class="flex flex-col gap-7">
    <div class="flex flex-col gap-2 text-center">
      <span class="text-jhc-orange text-xl font-medium">Testimonial</span>
      <h3 class="text-jhc font-semibold text-4xl">Apa Kata Mereka ?</h3>
    </div>
    <div class="grid md:grid-cols-3 gap-4">
      {#each testimonials as t}
        <div class="flex flex-col gap-2 shadow-md rounded-xl border border-gray-200 py-4 px-5">
          <blockquote class="text-lg italic font-medium leading-6 pb-2">
            {t.content}
          </blockquote>
          <div class="w-full h-1 border-dashed border-t border-jhc-orange"></div>
          <div class="flex flex-col justify-end gap-0 items-end">
            <span class="text-sm font-semibold">{t.name}</span>
            <span class="text-xs">{t.role}</span>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
