<script>
  import ServicesItem from "./ServicesItem.svelte";
  import {
    MusicNote,
    LightningBolt,
    Cake,
    Microphone,
  } from "svelte-hero-icons";
</script>

<section class="text-gray-700 body-font">
  <div
    class="container px- pt-24 mx-auto flex mb-12 items-center flex-wrap justify-center md:jusitfy-start">
    <div class="lg:max-w-lg lg:1/3 md:w-1/2 w-5/6">
      <img
        class="object-cover object-center w-full h-full"
        src="/assets/worker.svg"
        alt="stats" />
    </div>
    <div
      class="lg:flex-grow md:w-1/2 w-5/6 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center">
      <h1 class="title-section w-full">Your event needs always ensured</h1>
      <p class="subtitle-section w-full mb-8">
        There is always a team of professionals and quality material ready to
        ensure your event needs at a glance. You are going to save countless
        hours spent looking for the best team to fullfil your event's needs in
        the area. From sports to parties, we provide a huge set of services to
        all our clients, that are going to be crucial to the success of the
        event.
      </p>
    </div>
  </div>
  <div class="container px-5 pb-24 mx-auto flex">
    <div class="flex flex-wrap justify-center w-full">
      <div class="w-1/2 md:w-1/4 mb-6 md:mb-0">
        <ServicesItem
          title="SHOWS"
          icon={MusicNote}
          features={['Stage Team', 'Lights & Sound Team', 'Musical Instruments']} />
      </div>
      <div class="w-1/2 md:w-1/4 mb-6 md:mb-0">
        <ServicesItem
          title="PARTIES"
          icon={Cake}
          features={['Catering', 'Artists & Animators']} />
      </div>
      <div class="w-1/2 md:w-1/4">
        <ServicesItem
          title="SPORTS"
          icon={LightningBolt}
          features={['Sports Equipment']} />
      </div>
      <div class="w-1/2 md:w-1/4">
        <ServicesItem
          title="CONFERENCES"
          icon={Microphone}
          features={['Stage Team', 'Lights & Sound Team', 'Projectors']} />
      </div>
    </div>
  </div>
</section>
