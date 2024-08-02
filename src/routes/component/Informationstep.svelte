<script>
    import Informationcadre from "./utilities/Informationcadre.svelte";
</script>

<section>
    <div class="contenaire one">
        <div class="card">
            <Informationcadre
                title="01 Découvrez"
                paragraph1="Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian pork lot anchovies. Lovers crust chicken garlic style parmesan deep beef"
                paragraph2="Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian pork lot anchovies. Lovers crust chicken garlic style parmesan deep beef"
                srcimg="/src/assets/iaimage/red.png"
            /> 
        </div>
    </div>
    <div class="contenaire two">
        <div class="card">
            <Informationcadre
                title="02 Essayer"
                paragraph1="Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian pork lot anchovies. Lovers crust chicken garlic style parmesan deep beef"
                paragraph2="Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian pork lot anchovies. Lovers crust chicken garlic style parmesan deep beef"
                srcimg="/src/assets/iaimage/green.png"
            /> 
            
        </div> 
    </div>
    <div class="contenaire three">
        <div class="card">
             <Informationcadre
                title="03 Adoptez"
                paragraph1="Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian pork lot anchovies. Lovers crust chicken garlic style parmesan deep beef"
                paragraph2="Pizza ipsum dolor meat lovers buffalo. Ricotta bell mayo pie green Hawaiian pork lot anchovies. Lovers crust chicken garlic style parmesan deep beef"
                srcimg="/src/assets/iaimage/purple.png"
            /> 
           
        </div>
    </div>
</section>

<style>
    section {
        margin: 0 auto;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-content: space-between;
        width: 80%;
        max-width: 1250px;
    }

    .card {
        position: sticky;
        top: 10px; 
       
    }

    .contenaire {  
        display: flex;
        align-items: flex-start;
        justify-content: center; 
    }

    @media screen and (max-width: 1600px) {
        section {
            width: 90%;
            max-width: 100vw;
        }
    }

    @media screen and (max-width: 1370px) {
        section {
            width: 95%;
        }
    }

    @media screen and (max-width: 1300px) {
        section {
            flex-direction: column;
            gap: 24px;
        }
    }
</style>
