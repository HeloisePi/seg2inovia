<script>
  import ContactUs from "./component/ContactUs.svelte";
  import Footer from "./component/Footer.svelte";
  import Hero from "./component/Hero.svelte";
  import Informationstep from "./component/Informationstep.svelte";
  import Textzone from "./component/Textzone.svelte";
  import Opensite from "./component/utilities/Opensite.svelte";

</script>

<Opensite />
<Hero />
<div>
<Informationstep/>



<Textzone />
<ContactUs />
<Footer />

</div>

<style>
  div{
    display: flex;
    flex-direction: column;
    gap: 316px;
  }
</style>