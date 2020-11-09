<script lang="ts">
  import { Search } from "svelte-hero-icons";
  import TypingText from "../../../../components/TypingText/TypingText.svelte";
</script>

<section class="text-gray-700 body-font relative">
  <div
    class="relative container mx-auto flex px-5 py-24 md:flex-row flex-col items-center ">
    <div
      class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center">
      <h1 class="title-hero">
        A place to find and
        <br class="hidden lg:inline-block" />
        plan
        <TypingText
          delay={100}
          waitToDelete={1000}
          words={['sports games', 'shows', 'meetings', 'weddings', 'parties']} />
      </h1>
      <p class="subtitle-hero">
        Creating events is easier with Pland. Search throughout thousands of
        events occuring right now or create your own and invite your friends.
      </p>
      <div class="flex justify-center">
        <button class="btn btn-primary">Sign up</button>
        <button class="ml-4 btn btn-secundary ">Learn More</button>
      </div>
    </div>
    <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6 relative">
      <img
        class="object-cover object-center rounded relative z-10 w-full"
        alt="hero"
        src="/assets/party.svg" />
    </div>
  </div>
</section>
