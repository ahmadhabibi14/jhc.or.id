<script lang="ts">
  import { writable, type Writable } from 'svelte/store';
	import { Icon } from 'svelte-icons-pack';
	import { BsList } from 'svelte-icons-pack/bs';
	import { RiSystemCloseFill } from 'svelte-icons-pack/ri';

  const isShowMenu: Writable<Boolean> = writable(false);
</script>

<div id="top" class="top-0 z-99 fixed w-full h-20 flex flex-row items-center justify-center py-auto bg-white shadow-lg">
  <div class="px-5 md:px-0 container max-w-6xl flex flex-row items-center justify-between mx-auto">
    <div class="flex flex-row gap-3 items-center">
      <div class="flex md:hidden">
        <button
          type="button"
          onclick={() => $isShowMenu = !$isShowMenu}
          class="">
          <Icon
            src={BsList}
            size="30"
          />
        </button>
      </div>
      <a href="/" class="w-fit h-fit">
        <img
          src="/icons/logo-text.svg"
          alt="Jayakarta Halal Center"
          class="h-12 w-auto"
        />
      </a>
    </div>
    <nav class="hidden md:flex flex-row gap-8 items-center justify-center w-fit font-semibold">
      <a href="/" class="hover:text-jhc-orange">Beranda</a>
      <a href="/#tentang" class="hover:text-jhc-orange">Tentang Kami</a>
      <a href="/#paket" class="hover:text-jhc-orange">Paket</a>
      <a href="/#kontak" class="hover:text-jhc-orange">Kontak</a>
    </nav>
    <a
      href="https://wa.me/6281322482220"
      class="md:block hidden w-fit h-fit cursor-pointer py-3 px-6 rounded-full text-white bg-jhc hover:bg-jhc-2 text-sm"
    >
      Konsultasi Gratis
    </a>
  </div>
</div>

<aside
  class="{$isShowMenu ? 'left-0' : '-left-[250px]'} duration-150 py-6 px-6 h-dvh w-[250px] bg-black text-gray-300 rounded-r-xl
  fixed z-110 top-0 bottom-0 flex flex-col gap-5">
  <a
    class="hover:text-jhc  px-4 pt-1 pb-2 w-fit border-b-2"
    href="/"
    onclick={()=> $isShowMenu = false}
  >
    Beranda
  </a>
</aside>