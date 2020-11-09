<script>
  import ServicesItem from "./ServicesItem.svelte";
  import { UserGroup, Sparkles, Cog } from "svelte-hero-icons";
</script>

<section
  class="text-gray-700 body-font bg-gradient-to-b from-purple-100 to-indigo-100">
  <div class="container px-5 py-24 mx-auto">
    <div class="grid grid-cols-12 gap-4 sm:-m-4 -mx-4 -mb-10 -mt-4 px-6">
      <ServicesItem
        title="Events for everyone"
        icon={UserGroup}
        body="Whether you are an individual or a company, you can use Pland to promote your event ideas
            with your community or with new people that are ready to discover new ways to spend their time." />
      <ServicesItem
        title="New experiences near you"
        icon={Sparkles}
        body="If you are bored with your daily life, we have prepared a huge set of new possibilities that are going to open your mind and desires. Create your account today and find the best experiences around you." />
      <ServicesItem
        title="Your needs at a glance"
        icon={Cog}
        body="Choose what you need in your events easily, without having the trouble you used to. We provide a variety of resourceful and trustworthy services you can ask upon the event creation, always without leaving our application. " />
    </div>
  </div>
</section>
