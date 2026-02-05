<script lang="ts">
	import { Icon, type IconType } from "svelte-icons-pack";
	import { RiDeviceDatabase2Line, RiDocumentBookOpenLine, RiDocumentFileEditLine, RiDocumentFolderChartLine, RiOthersBox3Line, RiUserFacesTeamLine } from "svelte-icons-pack/ri";

  const benefits: {
    icon: IconType;
    content: string;
  }[] = [
    {
      icon: RiDeviceDatabase2Line,
      content: 'Dokumen Data Assessment'
    },
    {
      icon: RiDocumentBookOpenLine,
      content: 'Pendampingan Lapangan'
    },
    {
      icon: RiOthersBox3Line,
      content: 'Pengawalan Proses Produksi'
    },
    {
      icon: RiUserFacesTeamLine,
      content: 'Edukasi Tim Internal'
    },
    {
      icon: RiDocumentFileEditLine,
      content: 'Penyusunan SJPH manual'
    },
    {
      icon: RiDocumentFolderChartLine,
      content: 'Monitoring Evaluasi Pasca Sertifikasi'
    }
  ]
</script>

<section class="container max-w-6xl mx-auto my-16 md:px-5 lg:px-0 px-5" id="benefit">
  <div class="grid grid-cols-1 md:grid-cols-3 md:grid-rows-2 gap-5 w-full h-fit px-4 md:px-6 py-10 rounded-4xl bg-jhc text-white md:text-lg">
    {#each benefits as bnf}
      <div class="w-full flex flex-row items-center gap-3 bg-jhc-2 rounded-full py-2 md:px-4 px-3">
        <Icon
          src={bnf.icon}
          className="text-jhc-orange stroke-jhc-orange fill-jhc-orange w-6 md:w-10 h-auto shrink-0"
        />
        <span class="grow">{bnf.content}</span>
      </div>
    {/each}
  </div>
</section>