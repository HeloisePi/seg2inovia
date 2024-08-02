<script>
  import Whitebutton from "./utilities/Whitebutton.svelte";

</script>

<section>
    <h2>Contactez nous </h2>
    <p>Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian pork lot anchovies. Lovers crust chicken garlic style parmesan deep beef mushrooms marinara. Ham roll green dolor Chicago. </p>
    <Whitebutton href="#"><p>Linkedin</p></Whitebutton>
    <Whitebutton href="#"><p>Instagram</p></Whitebutton>
    <Whitebutton href="#"><p>Facebook</p></Whitebutton>
</section>




<style>
    section{
        display: flex;
        flex-direction: column;
        gap: 24px;
        width: 80%;
        margin: auto;
        max-width: 1250px;
    }
    p{
        max-width: 468px;
        width: 80%;
    }
</style>