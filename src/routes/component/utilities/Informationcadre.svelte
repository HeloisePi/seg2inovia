<!-- Informationcadre.svelte -->
<script>
    export let title;
    export let paragraph1;
    export let paragraph2;
    export let srcimg;

    let constrain = 200;
    let imgProjectContainer;

    let mouseX = 0;
    let mouseY = 0;

    function transforms(x, y, imgProject) {
        let calcX = -(y - imgProject.top - (imgProject.height / 2)) / constrain;
        let calcY = (x - imgProject.left - (imgProject.width / 2)) / constrain;
        return `perspective(150px) rotateX(${calcX}deg) rotateY(${calcY}deg)`;
    }

    function transformElement(el, xyEl) {
        let x = xyEl[0];
        let y = xyEl[1];
        let imgProject = xyEl[2];
        el.style.transform = transforms(x, y, imgProject);
    }

    let handleMouseMove = (e) => {
        mouseX = e.clientX;
        mouseY = e.clientY;

        let xy = [mouseX, mouseY];
        let imgProject = imgProjectContainer.getBoundingClientRect();
        let position = xy.concat([imgProject]);

        window.requestAnimationFrame(() => {
            transformElement(imgProjectContainer, position);
        });
    };

    let handleMouseLeave = () => {
        imgProjectContainer.style.transition = "transform 0.5s ease";
        imgProjectContainer.style.transform = "rotateX(0) rotateY(0)";
    };

    // Fonction retirée car nous n'avons plus besoin de mettre à jour l'arrière-plan
    // function updateHighlight(x, y, imgProject) {
    //     let relX = x - imgProject.left;
    //     let relY = y - imgProject.top;
    //     imgProjectContainer.style.background = `radial-gradient(circle at ${relX}px ${relY}px, rgba(30, 30, 30, 0.1), rgba(0, 0, 0, 0.6) 40%)`;
    // }
</script>

<section bind:this={imgProjectContainer} on:mousemove={handleMouseMove} on:mouseleave={handleMouseLeave} class="sticky-container">
    <div class="title">
        <h2>{title}</h2>
        <img src="/assets/arrow/seemore.svg" alt="seemore">
    </div>
    <div class="content">
        <p>{paragraph1}</p>
        <img class="illustration" src="{srcimg}" alt="image décorative ambiance ia">
        <p>{paragraph2}</p>
    </div>
</section>

<style>
    section {
        background: rgba(0, 0, 0, 0.60);
        border-radius: 10px;
        backdrop-filter: blur(6px);
        -webkit-backdrop-filter: blur(3.1px);
        border: 1px solid rgb(255, 255, 255);
        width: fit-content;
        position: sticky;
        top: 10px; /* Hauteur de l'espace sticky depuis le haut */
        overflow: visible; /* Assurez-vous que le contenu est visible */
        transition: transform 0.5s ease;
    }

    p, h2 {
        color: white;
    }

    .title {
        display: flex;
        justify-content: space-between;
        padding: 1.5rem;
        border-bottom: 1px solid white;
    }
    h2{
        max-width: 333px;
    }

    .content {
        padding: 1.5rem;
        max-width: 402px;
        display: flex;
        flex-direction: column;
        gap: 24px;
    }

    @media screen and (max-width: 430px) {
        .illustration{
            width: 100%;
            margin: auto;
        }
    }
</style>
