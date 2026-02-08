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
    }
  ];

  onMount(() => {
    const original = [...testimonials];
    while (testimonials.length < 12) {
      testimonials = [...testimonials, ...original.slice(0, 12 - testimonials.length)];
    }
  });
</script>

<section class="container max-w-6xl mx-auto my-16 md:px-5 lg:px-0 px-5" id="testimonials">
  <div class="flex flex-col gap-7">
    <div class="flex flex-col gap-2 text-center">
      <span class="text-jhc-orange text-xl font-medium">Testimonial</span>
      <h3 class="text-jhc font-semibold text-4xl">Apa Kata Mereka ?</h3>
    </div>
    <div class="flex justify-center items-center">
      <div class="w-full md:w-8/12 flex flex-col gap-2 shadow-md rounded-xl border border-gray-200 py-4 px-5 h-auto justify-between">
        <blockquote class="text-lg italic font-medium leading-6 pb-2">
          LPH Hidayatullah mengapresiasi kerja sama dengan Jayakarta Halal Center yang selama ini menunjukkan profesionalisme dan komitmen dalam mendukung layanan sertifikasi halal. Semoga sinergi ini terus berlanjut untuk memperkuat ekosistem halal yang terpercaya.
        </blockquote>
        <div class="flex flex-col gap-4">
          <div class="w-full h-1 border-dashed border-t border-jhc-orange"></div>
          <div class="flex flex-col justify-end gap-0 items-end">
            <span class="text-sm font-semibold">Muhammad Faisal</span>
            <p class="text-xs text-end">Ketua LPH Hidayatullah</p>
          </div>
        </div>
      </div>
    </div>
    <div class="testimonial-wrapper h-[270px]">
      {#each testimonials as t, idx}
        <div
          style="animation-delay: calc(50s / 6 * (6 - {idx+1}) * -1);"
          class="testimonial-item h-[260px]
          flex flex-col gap-2 shadow-md rounded-xl border border-gray-200
          py-4 px-5
          justify-between"
        >
          <blockquote class="italic font-medium leading-6 pb-2">
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
      {/each}
    </div>
  </div>
</section>

<style lang="postcss">
  @reference "tailwindcss";

  .testimonial-wrapper {
    width: 90%;
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

  @keyframes scrollLeft2Testimoni {
    to {
      left: -480px;
    }
  }

  .testimonial-item {
    width: 400px;
    position: absolute;
    left: max(calc(360px * 6), 100%);
    animation-name: scrollLeftTestimoni;
    animation-duration: 50s;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
  }
</style>