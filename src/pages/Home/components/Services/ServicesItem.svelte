<script lang="ts">
  export let title: string;
  export let body: string;
  export let icon: any;
</script>

<div
  class="col-span-12 md:col-span-4 w-full p-6 md:mb-0 mb-6 flex bg-white rounded-md">
  <div
    class="w-12 h-12 inline-flex items-center justify-center rounded-full bg-indigo-500 text-white mb-4 flex-shrink-0">
    <svelte:component this={icon} class="w-6" solid />
  </div>
  <div class="flex-grow pl-6">
    <h2 class="text-gray-900 text-lg title-font font-semibold mb-2">{title}</h2>
    <p class="leading-relaxed text-base text-gray-700 font-normal">{body}</p>
  </div>
</div>
