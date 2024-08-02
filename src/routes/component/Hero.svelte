<script>
  import Blackbutton from "./utilities/Blackbutton.svelte";

</script>


<section>
    <img class="logo" src="/assets/logo/logo.png" alt="Seg2Inov">
    <div class="testimage">
        <h1>L’intelligence artificielle pour les commerces </h1>
        <img class="illustration" src="/assets/iaimage/pink.jpg" alt="a painting blue">
    </div>
    
    
    <div class="navbar">
        <Blackbutton
        href="#"><p>Notre solution </p>
        </Blackbutton>
        <Blackbutton
        href="#">
            <p>S2cash</p>
        </Blackbutton>
        <Blackbutton
        href="#">
            <p>Nous contacter</p>
        </Blackbutton> 
    </div>
    
</section>

<style>
    section{
        margin: auto auto;
        width: 100vw;
        height: 95vh;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 34px;
        flex-direction: column;
        

    }

    .testimage{
        position: relative;
    }

    .logo{
        max-width: 318.65px;
        width: 25%;
        min-width: 168px;
    }

    p{
        color: white;
        z-index: 4;
        position: relative;
        font-size: 22px;
    }

    .navbar{
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 80%;
        max-width: 850px;
    }

    .illustration{
        position: absolute;
        right: 0;
        top: 0;
        z-index: -1;
        transform: translate(20%, -85%);
        max-height: 386px;
       
    }


    .white{
        color: white;
    }

    @media screen and (max-width: 800px) {
        .navbar{
            flex-direction: column;
            justify-content: center;
            align-items: flex-start;
            width: 318px;
            gap: 12px;

        }
        .illustration{
            display: none;
        }
        .white{
            color: black;
        }
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
        
        .illustration{
            transform: translate(30%, -72%);
            width: 106.76px;
            height: 187.32px;
            right: 0;
            display: none;
        }
        h1{
            max-width: 300px;
        }
    }

    @media screen and (max-width: 360px) {
        .illustration{
            transform: translate(2%, -152%);
            left: 0;
        }
    }

</style>