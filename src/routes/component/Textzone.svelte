<script></script>


<section>
    <div class="contenaire">
        <h2>Un commerce gagnant</h2>

        <p>L'étude des données de vente en temps réel permet de repérer les tendances, les comportements d'achat, les préférences des consommateurs et facilite la prise de décisions concernant les approvisionnements et la communication, marketing, promotions.<br>
            Disposer d'une connaissance approfondie des clients permet d’ajuster les stratégies commerciales, en mettant l'accent sur le programme de fidélité pertinent.<br>
            </p>
        <div class="contenaireab" ><div class="round"><h4>a</h4></div><p class="subtitle">Les recommandations basées sur l'IA peuvent être utiles aux vendeurs pour diriger les clients vers des produits alternatifs qu'ils n'auraient peut-être pas envisagés d'acheter.</p></div>
        <div class="contenaireab"><div class="round"><h4>b</h4></div><p class="subtitle">Les commerces peuvent recourir à l'IA pour diminuer le gaspillage, et les aider à augmenter leurs revenus et leurs marges en vérifiant que les articles sont en stock.        </p></div>
        <div class="contenaireab"><div class="round"><h4>c</h4></div><p class="subtitle">Les commerces ont la capacité d'utiliser l'IA pour examiner les données sur la demande, la concurrence et le coût des produits, afin de recommander des stratégies de tarification optimales.        </p></div>
    </div>
    <img src="/assets/iaimage/marketWin.png" alt="Ville pleine de couleure dans un style de peinture">
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