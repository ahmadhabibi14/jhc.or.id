<script lang="ts">
	import { Icon } from "svelte-icons-pack";
	import { RiSystemCheckboxCircleFill } from "svelte-icons-pack/ri";

  const productsGoods: string[] = [
    'Makanan dan Minuman',
    'Obat-obatan',
    'Kosmetik',
    'P. Rekayasa Genetik',
    'Barang gunaan'
  ];

  const productsServices: string[] = [
    'Penyembelihan',
    'Pengolahan',
    'Penyimpanan',
    'Pengemasan',
    'Pendistribusian',
    'Penjualan',
    'Penyajian'
  ]
</script>

<section class="container max-w-6xl mx-auto mb-16 mt-10 md:px-0 px-5" id="industry-usage">
  <div class="flex flex-col gap-7">
    <div class="flex flex-col gap-2 text-center">
      <span class="text-jhc-orange text-xl font-medium">Industri Halal</span>
      <h3 class="text-jhc font-semibold text-4xl">Produk Apa saja yang Wajib Bersertifikasi Halal ?</h3>
    </div>

    <div class="md:w-9/12 w-full mx-auto flex flex-col gap-5 md:grid grid-cols-2">
      <div class="w-full flex flex-col items-center gap-4 bg-jhc-2 rounded-2xl py-5 md:px-4 px-2 text-white">
        <h5 class="text-xl md:text-3xl font-semibold">Barang</h5>
        <div class="flex flex-col gap-1">
          {#each productsGoods as p}
            <div class="flex flex-row gap-2 items-center">
              <Icon
                src={RiSystemCheckboxCircleFill}
                size="18"
                className="text-jhc-orange fill-jhc-orange"
              />
              <p>{p}</p>
            </div>
          {/each}
        </div>
      </div>

      <div class="w-full flex flex-col items-center gap-4 bg-jhc-2 rounded-2xl py-5 md:px-4 px-2 text-white">
        <h5 class="text-xl md:text-3xl font-semibold">JASA</h5>
        <div class="flex flex-col gap-1">
          {#each productsServices as p}
            <div class="flex flex-row gap-2 items-center">
              <Icon
                src={RiSystemCheckboxCircleFill}
                size="18"
                className="text-jhc-orange fill-jhc-orange"
              />
              <p>{p}</p>
            </div>
          {/each}
        </div>
      </div>
    </div>
  </div>
</section>