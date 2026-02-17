<script lang="ts">
  import { onMount } from "svelte";

  let testimonials: {
    content: string;
    name: string;
    role: string;
  }[] = [
    {
      content:
        "Pendampingan sertifikasi halal untuk pabrik parfum kami berjalan cepat, rapi, dan jelas. Kini produk kami lebih siap bersaing di pasar nasional maupun ekspor.",
      name: "MICHAEL TAN",
      role: "Owner Pabrik Parfum, Pulo Gadung, Jakarta Timur"
    },
    {
      content:
        "Awalnya kami merasa pengurusan sertifikat halal itu rumit dan memakan waktu. Namun setelah didampingi, semua jadi lebih mudah dan jelas. Prosesnya cepat, komunikatif, dan sangat membantu kami sebagai pelaku usaha katering.",
      name: "RINDITYA",
      role: "Owner Katering Bandung, Jawa Barat"
    },
    {
      content:
        "Dengan sertifikat halal, kami merasa lebih tenang karena seluruh proses pengolahan makanan di restoran kami sudah sesuai regulasi halal pemerintah. Pendampingannya profesional dan mudah dipahami.",
      name: "JIHAD",
      role: "Owner Restoran Timur Tengah, Depok, Jawa Barat"
    },
    {
      content: "LPH Hidayatullah mengapresiasi kerja sama dengan Jayakarta Halal Center yang selama ini menunjukkan profesionalisme dan komitmen dalam mendukung layanan sertifikasi halal. Semoga sinergi ini terus berlanjut untuk memperkuat ekosistem halal yang terpercaya.",
      name: "MUHAMMAD FAISAL",
      role: "Ketua LPH Hidayatullah"
    },
    {
      content: "Sertifikat halal bukan hanya kepatuhan regulasi, tetapi lebih daripada itu adalah jaminan proses produksi agar sesuai syariah untuk menghasilkan daging halal. Dengan pendampingan dari JHC yang cepat, tepat dan akurat, kami semakin siap memenuhi kebutuhan pasar nasional bahkan internasional.",
      name: "Budi Susilo",
      role: "Pemilik RPH, Ciampea, Bogor"
    },
    {
      content:
        "Pendampingan sertifikasi halal untuk pabrik parfum kami berjalan cepat, rapi, dan jelas. Kini produk kami lebih siap bersaing di pasar nasional maupun ekspor.",
      name: "MICHAEL TAN",
      role: "Owner Pabrik Parfum, Pulo Gadung, Jakarta Timur"
    },
    {
      content:
        "Awalnya kami merasa pengurusan sertifikat halal itu rumit dan memakan waktu. Namun setelah didampingi, semua jadi lebih mudah dan jelas. Prosesnya cepat, komunikatif, dan sangat membantu kami sebagai pelaku usaha katering.",
      name: "RINDITYA",
      role: "Owner Katering Bandung, Jawa Barat"
    },
    {
      content:
        "Dengan sertifikat halal, kami merasa lebih tenang karena seluruh proses pengolahan makanan di restoran kami sudah sesuai regulasi halal pemerintah. Pendampingannya profesional dan mudah dipahami.",
      name: "JIHAD",
      role: "Owner Restoran Timur Tengah, Depok, Jawa Barat"
    },
    {
      content: "LPH Hidayatullah mengapresiasi kerja sama dengan Jayakarta Halal Center yang selama ini menunjukkan profesionalisme dan komitmen dalam mendukung layanan sertifikasi halal. Semoga sinergi ini terus berlanjut untuk memperkuat ekosistem halal yang terpercaya.",
      name: "MUHAMMAD FAISAL",
      role: "Ketua LPH Hidayatullah"
    },
    {
      content: "Sertifikat halal bukan hanya kepatuhan regulasi, tetapi lebih daripada itu adalah jaminan proses produksi agar sesuai syariah untuk menghasilkan daging halal. Dengan pendampingan dari JHC yang cepat, tepat dan akurat, kami semakin siap memenuhi kebutuhan pasar nasional bahkan internasional.",
      name: "Budi Susilo",
      role: "Pemilik RPH, Ciampea, Bogor"
    },


    {
      content:
        "Pendampingan sertifikasi halal untuk pabrik parfum kami berjalan cepat, rapi, dan jelas. Kini produk kami lebih siap bersaing di pasar nasional maupun ekspor.",
      name: "MICHAEL TAN",
      role: "Owner Pabrik Parfum, Pulo Gadung, Jakarta Timur"
    },
    {
      content:
        "Awalnya kami merasa pengurusan sertifikat halal itu rumit dan memakan waktu. Namun setelah didampingi, semua jadi lebih mudah dan jelas. Prosesnya cepat, komunikatif, dan sangat membantu kami sebagai pelaku usaha katering.",
      name: "RINDITYA",
      role: "Owner Katering Bandung, Jawa Barat"
    },
    {
      content:
        "Dengan sertifikat halal, kami merasa lebih tenang karena seluruh proses pengolahan makanan di restoran kami sudah sesuai regulasi halal pemerintah. Pendampingannya profesional dan mudah dipahami.",
      name: "JIHAD",
      role: "Owner Restoran Timur Tengah, Depok, Jawa Barat"
    },
    {
      content: "LPH Hidayatullah mengapresiasi kerja sama dengan Jayakarta Halal Center yang selama ini menunjukkan profesionalisme dan komitmen dalam mendukung layanan sertifikasi halal. Semoga sinergi ini terus berlanjut untuk memperkuat ekosistem halal yang terpercaya.",
      name: "MUHAMMAD FAISAL",
      role: "Ketua LPH Hidayatullah"
    },
    {
      content: "Sertifikat halal bukan hanya kepatuhan regulasi, tetapi lebih daripada itu adalah jaminan proses produksi agar sesuai syariah untuk menghasilkan daging halal. Dengan pendampingan dari JHC yang cepat, tepat dan akurat, kami semakin siap memenuhi kebutuhan pasar nasional bahkan internasional.",
      name: "Budi Susilo",
      role: "Pemilik RPH, Ciampea, Bogor"
    },
    {
      content:
        "Pendampingan sertifikasi halal untuk pabrik parfum kami berjalan cepat, rapi, dan jelas. Kini produk kami lebih siap bersaing di pasar nasional maupun ekspor.",
      name: "MICHAEL TAN",
      role: "Owner Pabrik Parfum, Pulo Gadung, Jakarta Timur"
    },
    {
      content:
        "Awalnya kami merasa pengurusan sertifikat halal itu rumit dan memakan waktu. Namun setelah didampingi, semua jadi lebih mudah dan jelas. Prosesnya cepat, komunikatif, dan sangat membantu kami sebagai pelaku usaha katering.",
      name: "RINDITYA",
      role: "Owner Katering Bandung, Jawa Barat"
    },
    {
      content:
        "Dengan sertifikat halal, kami merasa lebih tenang karena seluruh proses pengolahan makanan di restoran kami sudah sesuai regulasi halal pemerintah. Pendampingannya profesional dan mudah dipahami.",
      name: "JIHAD",
      role: "Owner Restoran Timur Tengah, Depok, Jawa Barat"
    },
    {
      content: "LPH Hidayatullah mengapresiasi kerja sama dengan Jayakarta Halal Center yang selama ini menunjukkan profesionalisme dan komitmen dalam mendukung layanan sertifikasi halal. Semoga sinergi ini terus berlanjut untuk memperkuat ekosistem halal yang terpercaya.",
      name: "MUHAMMAD FAISAL",
      role: "Ketua LPH Hidayatullah"
    },
    {
      content: "Sertifikat halal bukan hanya kepatuhan regulasi, tetapi lebih daripada itu adalah jaminan proses produksi agar sesuai syariah untuk menghasilkan daging halal. Dengan pendampingan dari JHC yang cepat, tepat dan akurat, kami semakin siap memenuhi kebutuhan pasar nasional bahkan internasional.",
      name: "Budi Susilo",
      role: "Pemilik RPH, Ciampea, Bogor"
    }
  ];
</script>

<section class="container max-w-6xl mx-auto my-16 md:px-5 lg:px-0 px-5 scroll-mt-20" id="testimonials">
  <div class="flex flex-col gap-7">
    <div class="flex flex-col gap-2 text-center">
      <span class="text-jhc-orange text-xl font-medium">Testimonial</span>
      <h3 class="text-jhc font-semibold text-4xl">Apa Kata Mereka ?</h3>
    </div>
    <div class="testimonial-wrapper h-[270px] group">
      {#each testimonials as t, idx}
        <div style="animation-delay: calc(50s / 6 * (6 - {idx+1}) * -1);"
        class="testimonial-item group-hover:[animation-play-state:paused]">
          <div
            class="h-[260px] w-full
            flex flex-col gap-2 shadow-md rounded-xl border border-gray-200
            py-4 px-5 bg-white
            justify-between z-10"
          >
            <blockquote class="italic font-medium leading-6 pb-2 line-clamp-6">
              {t.content}
            </blockquote>
            <div class="flex flex-col gap-4">
              <div class="w-full h-1 border-dashed border-t border-jhc-orange"></div>
              <div class="flex flex-col justify-end gap-0 items-end">
                <span class="text-sm font-semibold">{t.name}</span>
                <p class="text-xs text-end">{t.role}</p>
              </div>
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>

<style lang="postcss">
  @reference "tailwindcss";

  .testimonial-wrapper {
    width: 100%;
    max-width: 1536px;
    margin-inline: auto;
    position: relative;
    overflow: hidden;
    mask-image: linear-gradient(
      to right,
      rgba(0, 0, 0, 0),
      rgba(0, 0, 0, 1) 20%,
      rgba(0, 0, 0, 1) 80%,
      rgba(0, 0, 0, 0)
    );
  }

  @keyframes scrollLeftTestimoni {
    to {
      left: -400px;
    }
  }

  .testimonial-item {
    width: 400px;
    height: fit-content;
    position: absolute;
    left: max(calc(350px * 6), 100%);
    animation-name: scrollLeftTestimoni;
    animation-duration: 50s;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
  }
</style>