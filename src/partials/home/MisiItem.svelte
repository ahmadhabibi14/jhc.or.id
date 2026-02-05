<script lang="ts">
	import { Icon } from "svelte-icons-pack";
	import { FiPlusSquare, FiMinusSquare } from "svelte-icons-pack/fi";

  export let title: string = '';
  export let desc: string = '';

  let isShowDesc: boolean = false;
</script>

<div class="flex flex-row items-start gap-3">
  <button
    class="cursor-pointer mt-1"
    onclick={() => isShowDesc = !isShowDesc}
    aria-label="Toggle Description"
  >
    <Icon
      src={isShowDesc ?  FiMinusSquare : FiPlusSquare}
      size="18"
      className=""
    />
  </button>
  <div class="flex flex-col gap-0">
    <p class="font-medium">{title}</p>
    <div class="overflow-hidden
    transition-all
    duration-300
    ease-in-out
    max-h-0
    {isShowDesc ? 'max-h-96 mt-2' : ''}
    ">
      <p class="text-sm">{desc}</p>
    </div>
  </div>
</div>