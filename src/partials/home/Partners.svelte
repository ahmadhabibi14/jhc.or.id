<script lang="ts">
  const partners: {
    name: string;
    image: string;
  }[] = [
    {
      name: 'Pakocha',
      image: '/icons/partners/1.png',
    },
    {
      name: 'Rannur',
      image: '/icons/partners/2.png',
    },
    {
      name: 'AXL - Alexander',
      image: '/icons/partners/3.png',
    },
    {
      name: 'Pawon Ambu Jegger',
      image: '/icons/partners/4.png',
    },
    {
      name: 'Kebuli bin Jafar',
      image: '/icons/partners/5.png',
    },
    {
      name: 'SPPG',
      image: '/icons/partners/6.png',
    },
    {
      name: 'Bakmi Hejo',
      image: '/icons/partners/7.png',
    },
    {
      name: 'BWA - Boga Warisan Abbadi',
      image: '/icons/partners/8.png',
    },
    {
      name: 'One Man Show',
      image: '/icons/partners/9.png',
    },
    {
      name: 'MT Farm',
      image: '/icons/partners/10.png',
    },
    {
      name: 'Bentos',
      image: '/icons/partners/11.png',
    }
  ]
</script>

<section class="container max-w-6xl mx-auto mb-16 md:px-5 lg:px-0 px-5" id="partners">
  <div class="flex flex-col gap-7">
    <div class="flex flex-col gap-2 text-center">
      <span class="text-jhc-orange text-xl font-medium">Mitra Kami</span>
      <h3 class="text-jhc font-semibold text-4xl">Bersama Membangun Ekosistem Halal</h3>
    </div>
    <div class="partners-wrapper h-[120px] group">
      {#each partners as prt, idx}
        <div
          style="animation-delay: calc(20s / 6 * (6 - {idx+1}) * -1);"
          class="group-hover:[animation-play-state:paused] h-[120px] py-5 px-auto partner-item cursor-pointer flex justify-center items-center bg-white rounded-md"
          title={prt.name}
        >
          <img
            src={prt.image}
            alt=""
            class="w-auto h-full"
          />
        </div>
      {/each}
    </div>
  </div>
</section>

<style lang="postcss">
  @reference "tailwindcss";

  .partners-wrapper {
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

  @keyframes scrollLeftPartner {
    to {
      left: -200px;
    }
  }

  .partner-item {
    width: 200px;
    position: absolute;
    left: max(calc(170px * 6), 100%);
    animation-name: scrollLeftPartner;
    animation-duration: 20s;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
  }
</style>