<script>

</script>

<div class="div">
<section>
    <img class="logo" src="/assets/logo/logo.png" alt="Seg2Inov">

    <div class="contactlink">
        <h3>CONTACT</h3>
        <p>support@seg2inov.fr</p>
        <p>contact@seg2inov.fr</p>
        <p>09 70 70 36 96</p>
    </div>

    <div class="contactlink">
        <h3>OÙ NOUS TROUVER ?</h3>
        <div class="link"><p>LinkedIn</p> <img src="/assets/arrow/linkexterne.svg" alt="lien externe pour Linkedin"></div>
        <div  class="link" ><p>Facebook</p> <img src="/assets/arrow/linkexterne.svg" alt="lien externe pour facebook"></div>
        <div  class="link" ><p>Instagram</p> <img src="/assets/arrow/linkexterne.svg" alt="lien externe pour Instagram"></div>

    </div>
</section>
<div class="mentionlegale">
    <p>Mention Légal </p>
</div>
</div>







<style>
section{
    background-color: #EDEDED;
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 480px;

}

.link{
    display: flex;
    align-items: center;
    gap: 8px;
}

.contactlink{
    display: flex;
    flex-direction: column;
    gap: 24px;
}
.mentionlegale{
    background-color: #EDEDED;
    border-top: solid black 1px;
    display: flex;
    height: 50px;
    align-items: center;
    justify-content: center;

}

@media screen and (max-width: 920px) {

    section{
        flex-direction: column;
        height: fit-content;
        gap: 84px;
        align-items: start;
        padding: 15%;
    }
    .logo{
        width: 50%;
    }
}
</style>