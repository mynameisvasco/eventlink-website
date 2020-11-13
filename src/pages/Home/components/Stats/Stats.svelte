<script>
  import StatsItem from "./StatsItem.svelte";
  import { Users, Ticket, Home } from "svelte-hero-icons";
</script>

<section
  class="text-gray-700 body-font bg-gradient-to-b from-purple-100 to-indigo-100">
  <div class="container px-5 pt-12 pb-24 mx-auto flex flex-wrap">
    <div
      class="lg:w-1/2 sm:w-1/3 w-full rounded-lg overflow-hidden mt-6 sm:mt-0">
      <img
        class="object-cover object-center w-full h-full"
        src="/assets/rocket_boy.svg"
        alt="stats" />
    </div>
    <div
      class="flex flex-wrap mt-auto mb-auto lg:w-1/2 sm:w-2/3 content-start sm:pr-10">
      <div class="w-full sm:p-4 px-4 mb-2">
        <h1 class="title-section">
          Join the rocket today and help our community grow
        </h1>
        <div class="subtitle-section">
          Our main goal is to target more users and cities in order to make
          everyone's life easier when we are talking about find and plan events.
        </div>
      </div>
      <div class="w-1/2 md:w-1/3">
        <StatsItem name="Users" value="+10k" icon={Users} />
      </div>
      <div class="w-1/2 md:w-1/3">
        <StatsItem name="Events" value="+25k" icon={Ticket} />
      </div>
      <div class="w-1/2 md:w-1/3">
        <StatsItem name="Cities" value="2" icon={Home} />
      </div>
    </div>
  </div>
</section>
