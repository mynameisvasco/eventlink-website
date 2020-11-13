<script>
  import DownloadButton from "./DownloadButton.svelte";
</script>

<section class="text-gray-700 body-font">
  <div
    class="container mx-auto flex px-5 py-24 md:flex-row flex-col items-center">
    <div
      class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center">
      <h1 class="title-section">
        Your event with little effort, from anywhere.
      </h1>
      <p class="subtitle-section mb-8">
        Plan or find your desired event easily without the old troubles you were
        used to. You can do it with yur phone, tablet, laptop or any other
        device that is able to connect to internet.
      </p>
      <div class="flex lg:flex-row md:flex-col">
        <div class="mr-4 mb-0 md:mb-4">
          <DownloadButton type="google" />
        </div>
        <div class="mb-0 md:mb-4">
          <DownloadButton type="browser" />
        </div>
      </div>
    </div>
    <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6 order-first md:order-last">
      <img
        class="object-cover object-center rounded-md"
        alt="hero"
        src="/assets/calling.svg" />
    </div>
  </div>
</section>
