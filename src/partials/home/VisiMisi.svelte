<script>
	import { Icon } from "svelte-icons-pack";
	import { RiMediaRecordCircleLine } from "svelte-icons-pack/ri";
	import MisiItem from "./MisiItem.svelte";
</script>

<section class="container max-w-6xl mx-auto my-14 px-5 md:px-0" id="visi-misi">
  <div class="flex flex-col md:grid md:grid-cols-2 gap-5 md:gap-10">
    <div class="flex flex-row items-start gap-3 md:gap-6">
      <div class="flex justify-center items-center md:p-3 p-1.5 rounded-md bg-jhc-light text-jhc">
        <Icon
          src={RiMediaRecordCircleLine}
          className="md:w-10 w-5 h-auto"
        />
      </div>
      <div class="flex flex-col gap-3">
        <h3 class="text-2xl md:text-4xl font-bold text-jhc">Visi</h3>
        <p>Menjadi pusat layanan fasilitasi sertifikasi dan edukasi halal yang terpercaya dan berdaya saing global, serta berkontribusi dalam mewujudkan kehidupan yang sesuai prinsip syariah.</p>
      </div>
    </div>
    <div class="flex flex-row items-start gap-3 md:gap-6">
      <div class="flex justify-center items-center md:p-3 p-1.5 rounded-md bg-jhc-light text-jhc">
        <Icon
          src={RiMediaRecordCircleLine}
          className="md:w-10 w-5 h-auto"
        />
      </div>
      <div class="flex flex-col gap-3">
        <h3 class="text-2xl md:text-4xl font-bold text-jhc">Misi</h3>
        <div class="flex flex-col gap-2">
          <MisiItem
            title="Menyediakan Layanan Sertifikasi Halal yang Kredibel dan Profesional"
            desc="Memberikan layanan sertifikasi halal yang cepat, akurat, dan sesuai standar internasional. Menjamin transparansi dan kepercayaan dalam setiap proses sertifikasi."
          />
          <MisiItem
            title="Meningkatakan Kesadaran dan Pemahaman tentang Halal"
            desc="Menyelenggarakan program edukasi, pelatihan, dan kampanye kesadaran halal bagi masyarakat dan industri. Mendorong penerapan prinsip halal di berbagai aspek kehidupan."
          />
          <MisiItem
            title="Memperluas Jaringan dan Kerja Sama Strategis"
            desc="Membangun kemitraan dengan lembaga pemerintah, swasta, dan komunitas nasional dan internasional. Mendukung pertumbuhan industri halal melalui sinergi antar pemangku kepentingan."
          />
          <MisiItem
            title="Mewujudkan Tata Kelola yang Profesional dan Amanah"
            desc="Mengelola Jayakarta Halal Center dengan prinsip transparansi, akuntabilitas, dan keadilan. Meningkatkan kompetensi sumber daya manusia untuk mendorong operasional yang unggul."
          />
        </div>
      </div>
    </div>
  </div>
</section>