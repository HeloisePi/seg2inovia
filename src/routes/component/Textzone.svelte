<script></script>


<section>
    <div class="contenaire">
        <h2>LOREM ipsum titre </h2>

        <p>Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian pork lot anchovies. Lovers crust chicken garlic style parmesan deep beef mushrooms marinara. Ham roll green dolor Chicago. </p>
        <div class="contenaireab" ><div class="round"><h4>a</h4></div><p class="subtitle">Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian</p></div>
        <div class="contenaireab"><div class="round"><h4>b</h4></div><p class="subtitle">Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian</p></div>
        <div class="contenaireab"><div class="round"><h4>c</h4></div><p class="subtitle">Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian</p></div>
    </div>
    <img src="/assets/coverimage.svg" alt="">
</section>



<style>
    section{
        display: flex;
        width: 80%;
        max-width: 1250px;
        margin: auto;
        justify-content: space-between;
        gap: 92px;
    }

    .contenaire{
        display: flex;
        flex-direction: column;
        gap: 24px;
    }

    .round{
        border-radius: 50%;
        border: 1px solid black;
        width: 82px;
        height: 82px;
        display: flex;
        justify-content: center;
        align-items: center; 
    }

    .contenaireab{
        display: flex;
        gap: 24px;
        align-items: center;
    }

    p{
        max-width: 472px;
    }

    .subtitle{
        max-width: 354px;
        width: 80%;
    }

    @media screen and (max-width: 1485px) {
        .round{
            width: 50px;
            height: 50px;
        }

        img{
            width: 50%;
        }
    }

    @media screen and (max-width: 1300px) {
        img{
            width: 40%;
        }
    }
    @media screen and (max-width: 1100px) {
        section{
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        img{
            width: 80%;
        }
    }

    @media screen and (max-width: 540px) {
        .round{
            width: 37px;
            height: 37px;
        }

        .subtitle{
            width: 80%;
        }
    
    }
</style>