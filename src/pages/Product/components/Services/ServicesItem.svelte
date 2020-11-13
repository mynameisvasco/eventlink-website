<script lang="ts">
  export let title: string;
  export let features: string[];
  export let icon: any;
</script>

<div class="w-full">
  <h2
    class="flex items-center font-medium tracking-widest text-gray-900 mb-4 text-sm sm:text-left">
    <svelte:component this={icon} class="w-5 h-5 mr-1" solid />
    {title}
  </h2>
  <nav class="flex flex-col sm:items-start sm:text-left  -mb-1">
    {#each features as feat}
      <span class="mb-2">
        <span
          class="bg-indigo-100 text-indigo-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center">
          <svg
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="3"
            class="w-3 h-3"
            viewBox="0 0 24 24">
            <path d="M20 6L9 17l-5-5" />
          </svg>
        </span>
        {feat}
      </span>
    {/each}
  </nav>
</div>
