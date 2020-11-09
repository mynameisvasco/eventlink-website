<script>
  import OurTeamItem from "./OurTeamItem.svelte";
</script>

<section class="text-gray-700 body-font ">
  <div class="container px-5 py-24 mx-auto">
    <div class="flex flex-col text-center w-full mb-20">
      <h1 class="text-2xl font-medium title-font mb-4 text-gray-900">
        OUR TEAM
      </h1>
      <p class="lg:w-2/3 mx-auto leading-relaxed text-base">
        Meet the people who are behind this idea and that put their daily effort
        , always with the goal of providing you with the best experience
        possible.
      </p>
    </div>
    <div class="flex flex-wrap -m-4">
      <OurTeamItem
        name="Vasco Sousa"
        description="A passionate full stack developer, who is loooking for build smart solutions to hard daily problems."
        image="/assets/vasco.jpg"
        role="Developer" />
      <OurTeamItem
        name="Francisco Monteiro"
        description="A passionate full stack developer, who is loooking for build smart solutions to hard daily problems."
        image="/assets/vasco.jpg"
        role="Developer" />
      <OurTeamItem
        name="Ana Ferreira"
        description="A passionate full stack developer, who is loooking for build smart solutions to hard daily problems."
        image="/assets/vasco.jpg"
        role="Developer" />
      <OurTeamItem
        name="Sofia Vaz"
        description="A passionate full stack developer, who is loooking for build smart solutions to hard daily problems."
        image="/assets/vasco.jpg"
        role="Developer" />
    </div>
  </div>
</section>
