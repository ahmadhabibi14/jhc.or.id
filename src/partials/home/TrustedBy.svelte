<script>
	import { Icon } from "svelte-icons-pack";
	import { RiSystemCheckboxCircleFill } from "svelte-icons-pack/ri";

</script>
<div class="container max-w-6xl mx-auto my-7" id="dipercaya">
  <div class="flex flex-col gap-10">
    <div class="flex flex-col gap-2 text-center justify-center items-center">
      <span class="text-jhc-orange text-xl font-medium">Sertifikasi Resmi Melalui</span>
      <h3 class="text-jhc font-semibold text-4xl">Dipercaya Pelaku Usaha, Diakui Negara.</h3>
    </div>
    <div class="grid grid-cols-2">
      <div class="flex flex-col gap-7">
        <p>Bergabunglah dengan jaringan pengusaha yang telah sukses naik kelas. Kami mengawal ketat standarisasi halal untuk memastikan brand Anda memiliki keunggulan kompetitif di pasar dengan label Halal resmi.</p>
        <div class="flex flex-col gap-1 text-jhc-2">
          <div class="flex flex-row gap-2 items-center">
            <Icon
              src={RiSystemCheckboxCircleFill}
              size="18"
              className="text-jhc-orange fill-jhc-orange"
            />
            <p>Spesialis Pendampingan Unit Gizi & MBG</p>
          </div>
          <div class="flex flex-row gap-2 items-center">
            <Icon
              src={RiSystemCheckboxCircleFill}
              size="18"
              className="text-jhc-orange fill-jhc-orange"
            />
            <p>Solusi Sertifikasi Lintas Industri</p>
          </div>
          <div class="flex flex-row gap-2 items-center">
            <Icon
              src={RiSystemCheckboxCircleFill}
              size="18"
              className="text-jhc-orange fill-jhc-orange"
            />
            <p>Jaminan Kriteria BPJPH</p>
          </div>
        </div>
      </div>
      <div class="bpjhp-container rounded-2xl flex justify-center items-center h-[300px]">
        <img
          src="/img/cert-bpjph.png"
          alt="BPJHP"
          class="h-full w-auto"
        />
      </div>
    </div>
  </div>
</div>

<style>
  .bpjhp-container {
    border: 2px solid rgba(27, 91, 95, 1);
    box-shadow: 6px 6px 0px 0px rgba(27, 91, 95, 1);
    -webkit-box-shadow: 6px 6px 0px 0px rgba(27, 91, 95, 1);
  }
</style>