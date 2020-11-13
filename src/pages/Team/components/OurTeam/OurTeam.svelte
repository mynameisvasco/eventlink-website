<script>
  import OurTeamItem from "./OurTeamItem.svelte";
</script>

<section class="text-gray-700 body-font ">
  <div class="container px-5 py-24 mx-auto">
    <div class="flex flex-col text-center w-full mb-20">
      <h1 class="title-section">Our Team</h1>
      <p class="lg:w-2/3 mx-auto subtitle-section">
        Meet the people who are behind this idea and that put their daily effort
        , always with the goal of providing you with the best experience
        possible.
      </p>
    </div>
    <div class="flex flex-wrap -m-4">
      <OurTeamItem
        name="Vasco Sousa"
        description="A passionate full stack developer, who is loooking to build smart solutions to hard daily problems."
        image="/assets/vasco.jpg"
        role="Developer" />
      <OurTeamItem
        name="Francisco Monteiro"
        description="A young and bright star of engineering, who solves real life problems through technological approaches."
        image="/assets/francisco.jpg"
        role="Developer" />
      <OurTeamItem
        name="Ana Ferreira"
        description="A tiny developer."
        image="/assets/ana.jpg"
        role="Developer" />
      <OurTeamItem
        name="Sofia Vaz"
        description="Books and ones and zeros are some of the things that keep me busy."
        image="/assets/sofia.png"
        role="Developer" />
    </div>
  </div>
</section>
