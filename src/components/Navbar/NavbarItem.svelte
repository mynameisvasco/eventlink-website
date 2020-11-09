<script lang="ts">
  import { Link } from "svelte-routing";
  export let name: string;
  export let link: string;

  let isActive = false;
</script>

<Link
  to={link}
  getProps={({ location, href, isPartiallyCurrent, isCurrent }) => (isActive = isCurrent)}>
  <span
    class:text-indigo-500={isActive}
    class="cursor-pointer mr-5 hover:text-gray-900 font-medium">{name}</span>
</Link>
