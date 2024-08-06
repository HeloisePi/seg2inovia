<script>
  import Whitebutton from "./utilities/Whitebutton.svelte";

</script>

<section class="contenaire">
    <h2>Contactez nous </h2>
    <p>Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian pork lot anchovies. Lovers crust chicken garlic style parmesan deep beef mushrooms marinara. Ham roll green dolor Chicago. </p>
    <div class="linkedin ">
        <img class="linkedinimg img" src="/assets/linkedin.png" alt="linkedin">
        <Whitebutton href="https://www.linkedin.com/company/seg2inov/?viewAsMember=true"><p>Linkedin</p></Whitebutton>
    </div>
    <div class="facebook ">
        <img class="facebookimg img" src="/assets/instagram.png" alt="image instagram">
        <Whitebutton href="https://www.instagram.com/seg2inov/"><p>Instagram</p></Whitebutton>
    </div>
    <div class="instagram ">
        <img class="instagramimg img" src="/assets/facebook.png" alt="image facebook">
        <Whitebutton href="https://www.facebook.com/profile.php?id=61562257696981"><p>Facebook</p></Whitebutton>
    </div> 
</section>




<style>

    .contenaire{
        position: relative;
    }


    .img{
        opacity:0;
        position: absolute;
        right: 0;
        bottom: 0;
        width: 613px;
        height: 473px;
        object-fit: scale-down;
        transition: 500ms ease-in-out;
    }

    .linkedin:hover .linkedinimg {
        opacity: 1;
    }

    .facebook:hover .facebookimg {
        opacity: 1;
    }

    .instagram:hover .instagramimg {
        opacity: 1;
    }

    section{
        display: flex;
        flex-direction: column;
        gap: 44px;
        width: 80%;
        margin: auto;
        max-width: 1250px;
    }
    p{
        max-width: 468px;
        width: 80%;
    }



    @media screen and (max-width: 1368px) {
        .img{
            width: 50%;
            height: fit-content;
        }
    }

    @media screen and (max-width: 911px) {
       .img{
       
        height: fit-content;
        transform: translateY(120%);
        left: 0;
        min-width: 290;
       }
    
    }
    
</style>