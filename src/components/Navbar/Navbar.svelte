<script>
  import NavbarItem from "./NavbarItem.svelte";

  let scrollY = 0;
  let scrollCssClass = "bg-transparent";

  $: {
    if (scrollY > 50) {
      scrollCssClass = "bg-white z-20 border-b border-gray-400";
    } else {
      scrollCssClass = "bg-transparent";
    }
  }
</script>

<svelte:window bind:scrollY />
<div class="pb-12">
  <header
    class="{scrollCssClass} fixed text-gray-700 body-font w-full z-30 transition-all duration-300 ease-in-out">
    <div
      class="container mx-auto flex flex-wrap p-5 flex-col md:flex-row items-center ">
      <span
        class="flex title-font font-medium items-center text-gray-900 mb-4 md:mb-0">
        <img src="/assets/logo.png" class="w-10" alt="logo" />
        <span class="ml-3 text-xl">Pland</span>
      </span>
      <nav
        class="md:mr-auto md:ml-4 md:py-1 md:pl-4 md:border-l md:border-gray-400	flex flex-wrap items-center text-base justify-center">
        <NavbarItem name="Home" link="/" />
        <NavbarItem name="Product" link="/product" />
        <NavbarItem name="Team" link="/team" />
        <NavbarItem name="Documentation" link="/docs" />
      </nav>
    </div>
  </header>
</div>
