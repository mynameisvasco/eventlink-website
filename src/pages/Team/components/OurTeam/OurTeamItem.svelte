<script lang="ts">
  export let name: string;
  export let role: string;
  export let description: string;
  export let image: string;
</script>

<div class="p-4 lg:w-1/4 md:w-1/2">
  <div class="h-full flex flex-col items-center text-center">
    <img
      alt="team"
      class="flex-shrink-0 rounded-lg w-full h-56 object-cover object-center mb-4"
      src={image} />
    <div class="w-full">
      <h2 class="title-font font-semibold text-lg text-gray-900">{name}</h2>
      <h3 class="text-gray-500 mb-3">{role}</h3>
      <p class="mb-4 text-gray-700">{description}</p>
    </div>
  </div>
</div>
