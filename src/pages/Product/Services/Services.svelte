<script>
  import ServicesItem from "./ServicesItem.svelte";
  import { MusicNote } from "svelte-hero-icons";
</script>

<section class="text-gray-700 body-font">
  <div class="container px-5 py-24 mx-auto">
    <div class="text-center mb-20">
      <h1 class="title-section">Your event needs always ensured</h1>
      <p class="subtitle-section mx-auto w-2/3">
        There is always a team of professionals and quality material ready to
        ensure your event needs at a glance. You are going to save countless
        hours spent looking for the best team to fullfil your event's needs in
        the area.
      </p>
    </div>
    <div class="flex flex-wrap lg:w-4/5 sm:mx-auto sm:mb-2 -mx-2 ">
      <div class="w-full ml-2 text-base font-semibold text-gray-500">
        <h2 class="flex items-center">
          <MusicNote class="w-5 h-5 mr-1" solid />
          Shows & Parties
        </h2>
      </div>
      <ServicesItem text="Stage Equipment" />
      <ServicesItem text="Animators/Artists" />
      <ServicesItem text="Lights/Sound Team" />
      <ServicesItem text="Musical Instruments" />
      <div class="w-full ml-2 text-base font-semibold text-gray-500 mt-8">
        <h2 class="flex items-center">
          <MusicNote class="w-5 h-5 mr-1" solid />
          Sports
        </h2>
      </div>
      <ServicesItem text="Stage Equipment" />
      <ServicesItem text="Animators/Artists" />
      <ServicesItem text="Lights/Sound Team" />
      <ServicesItem text="Musical Instruments" />
    </div>
  </div>
</section>
