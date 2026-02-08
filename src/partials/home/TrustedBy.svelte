<script lang="ts">
	import { Icon } from "svelte-icons-pack";
	import { RiSystemCheckboxCircleFill } from "svelte-icons-pack/ri";

  const features: string[] = [
    'UMKM industri pengolahan makanan dan minuman',
    'Satuan Pelayanan Pemenuhan Gizi (SPPG) MBG',
    'Restoran dan cafe',
    'Katering',
    'Pabrik kosmetik',
    'Jasa Penyembelihan Rumah Potong Hewan',
    'Dan lain sebagainya'
  ]
</script>

<section class="container max-w-6xl mx-auto my-16 md:px-0 px-5" id="dipercaya">
  <div class="flex flex-col gap-10">
    <div class="flex flex-col gap-2 text-center justify-center items-center">
      <span class="text-jhc-orange text-xl font-medium">Sertifikasi Resmi Melalui</span>
      <h3 class="text-jhc font-semibold text-4xl">Dipercaya Pelaku Usaha, Diakui Negara.</h3>
    </div>
    <div class="md:grid md:grid-cols-2 flex flex-col gap-5">
      <div class="flex flex-col gap-4">
        <p>
          Bergabunglah dengan jaringan pengusaha yang telah sukses naik kelas. Kami mengawal mulai dari tahap persiapan hingga evaluasi Penerapan Sistem Jaminan Produk Halal untuk memastikan brand Anda memiliki keunggulan kompetitif di pasar dengan label Halal resmi BPJPH.  
        </p>
        <p>
          Telah membantu Fasilitasi Pengurusan Sertifikat Halal:
        </p>
        <div class="flex flex-col gap-1 text-jhc-2">
          {#each features as feature}
            <div class="flex flex-row gap-2 items-center">
              <Icon
                src={RiSystemCheckboxCircleFill}
                size="18"
                className="text-jhc-orange fill-jhc-orange"
              />
              <p>{feature}</p>
            </div>
          {/each}
        </div>
      </div>
      <div class="bpjhp-container md:rounded-2xl flex justify-center items-center md:h-[200px] lg:h-[300px] w-full h-auto">
        <img
          src="/img/cert-bpjph.png"
          alt="BPJHP"
          class="h-full w-auto"
        />
      </div>
    </div>
  </div>
</section>

<style>
  .bpjhp-container {
    border: 2px solid rgba(27, 91, 95, 1);
    box-shadow: 6px 6px 0px 0px rgba(27, 91, 95, 1);
    -webkit-box-shadow: 6px 6px 0px 0px rgba(27, 91, 95, 1);
  }

  @media screen and (max-width: 768px) {
    .bpjhp-container {
      border: none;
      box-shadow: none;
      -webkit-box-shadow: none;
    }
  }
</style>