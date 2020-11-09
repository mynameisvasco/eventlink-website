<script lang="ts">
  export let name: string;
  export let value: string;
  export let icon: any;
</script>

<div class="p-4 sm:w-1/3 lg:w-1/3 w-1/3 flex items-center">
  <div
    class="w-12 h-12 mr-3 inline-flex items-center justify-center rounded-full bg-indigo-500 text-white flex-shrink-0">
    <svelte:component this={icon} class="w-6" solid />
  </div>

  <div>
    <h2 class="font-medium text-3xl text-gray-900">{value}</h2>
    <p class="leading-relaxed">{name}</p>
  </div>
</div>
