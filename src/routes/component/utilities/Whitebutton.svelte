<script>
    export let href;
</script>


<a href={href}>
    <slot>
    </slot>

    <img src="/assets/arrow/send.svg" alt="Aller sur le reseau">
</a>


<style lang="scss">
    @import '../../../style/main.scss';
    a{
        border-radius: 30px;
        border: 1px solid black;
        padding: 28px;
        padding-left: 37px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 320px;  
    }

    a:hover img{  
        transform: translateX(12px);
            
    }

    img{
        transition: 200ms ease-in;
    }


    @media screen and (max-width: 430px) {
        a{
        width: 80%;  
        padding: 20px;

    }

    
    }



</style>