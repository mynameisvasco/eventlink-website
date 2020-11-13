<script lang="ts">
  export let headers: string[];
  export let title: string;
</script>

{#if title}
  <div class="mb-2">
    <span class="text-1xl font-medium text-gray-900">{title}</span>
  </div>
{/if}
<table
  class="table-auto w-full text-left whitespace-no-wrap border border-gray-200">
  <thead>
    <tr>
      {#each headers as header}
        <th
          class="px-4 py-3 title-font tracking-wider font-medium text-gray-900 text-sm bg-gray-200 rounded-tl rounded-bl">
          {header}
        </th>
      {/each}
    </tr>
  </thead>
  <tbody>
    <slot />
  </tbody>
</table>
