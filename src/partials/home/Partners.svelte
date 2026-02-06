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
    }
  ]
</script>

<section class="container max-w-6xl mx-auto mb-16 md:px-5 lg:px-0 px-5" id="partners">
  <div class="flex flex-col gap-7">
    <div class="flex flex-col gap-2 text-center">
      <span class="text-jhc-orange text-xl font-medium">Mitra Kami</span>
      <h3 class="text-jhc font-semibold text-4xl">Bersama Membangun Ekosistem Halal</h3>
    </div>
    <div class="flex flex-wrap gap-6 md:gap-8 lg:gap-10 justify-center items-center">
      {#each partners as p}
        <div class="h-[120px] w-auto">
          <img
            src={p.image}
            alt={p.name}
            title={p.name}
            class="object-cover w-full h-full cursor-pointer"
          />
        </div>
      {/each}
    </div>
  </div>
</section>