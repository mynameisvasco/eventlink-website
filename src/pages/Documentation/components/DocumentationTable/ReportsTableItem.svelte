<script lang="ts">
  export let name: string;
  export let version: string;
  export let link: string;
</script>

<tr>
  <td class="px-4 py-3">{name}</td>
  <td class="px-4 py-3 text-indigo-500">
    <a href={link} target="_blank" alt={name + version}>{version}</a>
  </td>
</tr>
