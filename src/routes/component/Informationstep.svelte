<script>
    import Informationcadre from "./utilities/Informationcadre.svelte";
</script>

<section>
    <div class="contenaire one">
        <div class="card">
            <Informationcadre
                title="01 Mieux comprendre son marché"
                paragraph1="La compréhension de l'environnement de vente d'un produit est améliorée grâce à l'intelligence artificielle. En analysant les données clients, l'IA peut identifier les préférences et les comportements d'achat des consommateurs, ce qui permet aux entreprises de mieux cibler leurs offres et de répondre aux attentes du marché. La pertinence des données permet aux commerces d'ajuster leurs prix en temps réel pour maximiser leurs revenus tout en restant compétitifs."
                paragraph2="L'automatisation permet à l'IA d'optimiser les opérations de communication et de proposer des interactions, tout en proposant des offres personnalisées. Les commerces renforcent leur relation client en analysant les données clients et en offrant une expérience de proximité plus qualitative."
                srcimg="/assets/iaimage/knowMarquet.png"
            /> 
        </div>
    </div>
    <div class="contenaire two">
        <div class="card">
            <Informationcadre
                title="02 Fidéliser ses clients"
                paragraph1="L'intelligence artificielle permet de fidéliser les clients d'un magasin en créant une expérience unique entre les canaux physiques et digitaux. Élaboration de recommandations personnalisées pour les produits en utilisant les historiques de vente, automatisation et accélération des interactions avec les clients."
                paragraph2="L'IA contribue de manière significative à l'innovation des commerces en offrant une expérience d'achat fluide et cohérente. Elle favorise l'enrichissement du parcours d'achat tout en améliorant la satisfaction client."
                srcimg="/assets/iaimage/client.png"
            /> 
            
        </div> 
    </div>
    <div class="contenaire three">
        <div class="card">
             <Informationcadre
                title="03  Optimisation des Processus avec l'IA"
                paragraph1="L’intelligence artificielle transforme la gestion des commerces en optimisant la chaîne d’approvisionnement et l’organisation des entrepôts. En prévoyant la demande, elle ajuste les stocks pour éviter les surcharges ou ruptures, tout en garantissant la disponibilité des produits."
                paragraph2="Grâce à l’analyse des données et à l’apprentissage automatique, l’IA améliore l’agencement des entrepôts, accélère la préparation des commandes et réduit les erreurs. Elle détecte également les problèmes logistiques en temps réel, permettant une réaction rapide pour maintenir l’efficacité opérationnelle."
                srcimg="/assets/iaimage/optimisation.png"
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
        max-width: 1650px;
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
