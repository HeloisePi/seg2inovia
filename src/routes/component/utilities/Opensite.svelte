<script></script>




<div>
    <img src="/assets/logo/logo.png" alt="SEG2INOV">
</div>




<style>
    div{
        width: 100vw;
        height: 100vh;
        background-color: #E7E7E7;
        /* opacity: 0; */
        position: fixed;
        top: 0;
        right: 0;
        animation: Apparition 2000ms;
        z-index: 100;
        display: flex;
        justify-content: center;
        align-items: center;
        transform: translateY(-100%);
        
    }

    img{
        width: 20%;
        height: auto;
        animation: Logo 2000ms ease-in-out;

    }



    @keyframes Logo{
       0%{
           opacity: 0;
       }



       50%{
        opacity: 1;
       }


       /* 72%{
        opacity: 0;
       }

       100%{
        opacity: 0;
       } */
    }





    @keyframes Apparition{
       0%{
            opacity: 1;
            transform: translateY(0%);
       }
       
       60%{
        opacity: 1;
        transform: translateY(0%);
       }

       100%{
            /* opacity: 0; */
            transform: translateY(-100%);
       }
    }

</style>