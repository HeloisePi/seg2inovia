<script>
  import Blackbutton from "./utilities/Blackbutton.svelte";
  import Whitebutton from "./utilities/Whitebutton.svelte";


</script>


<section>
    <h1>L’intelligence artificielle <br> de <span><img class="logo" src="/assets/logo/logo.png" alt="Seg2INov"></span> au service<br>
        des commerces.</h1>

    <Whitebutton href="#">
        <p>Notre solution</p>
    </Whitebutton>

    <Whitebutton href="#">
        <p>S2cash</p>
    </Whitebutton>
    
</section>

<style>
    section{
        margin: auto auto;
        width: 100vw;
        height: 95vh;
        display: flex;
        justify-content: flex-start;
        align-items: flex-start;
        gap: 54px;
        flex-direction: column;
        padding-top: 5%;
        padding-left: 10%;
        

    }

   

    .logo{
        max-width: 318.65px;
        width: 25%;
        transform: translateY(20px);
    }

    p{
        
        z-index: 4;
        position: relative;
        font-size: 22px;
    }





  
        
     @media screen and (max-width: 500px) {
        section{

            justify-content: center;
            align-items: flex-start;
            gap: 34px;
            padding-left: 10%;
        }
        p{
            font-size: 18px;
        }
        
       
        h1{
            max-width: 300px;
        }
    }


    @media screen and (max-width: 1300px) {
        .logo{
            height: 60px;
            transform: translateY(13px);
        }
    }

    @media screen and (max-width: 830px) {
        .logo{
            transform: translateY(10px);
            width: 25%;
            height: auto ;
        }
    }
    @media screen and (max-width: 550px) {
        .logo{
            height: 30px;
            transform: translateY(5px);
            height: auto;
            width: 35%;
        }
    }


</style>