<script lang="ts">
  export let date: string;
  export let version: string;
  export let author: string;
  export let changes: string;
</script>

<tr>
  <td class="px-4 py-3">{version}</td>
  <td class="px-4 py-3">{date}</td>
  <td class="px-4 py-3">{author}</td>
  <td class="px-4 py-3">{changes}</td>
</tr>
