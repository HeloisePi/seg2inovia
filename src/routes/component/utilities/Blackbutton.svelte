<script>
    export let href;
</script>

<a href="{href}"><slot></slot></a>


<style lang="scss">
    a{
        background-color: #252D2F;
        border-radius: 30px;
        padding: 12px;
        width: fit-content;
        display: block;
        position: relative;
        overflow: hidden;
        padding-left: 34px;
        padding-right: 34px;
       

    }

   
 

    a::after{
        content: url(/assets/iaimage/blue.jpg) ;
        height: 0;
        left: 0%;
        transition: all 250ms cubic-bezier(0.565, 0.020, 0.495, 0.990); /* custom */
        
        border-radius: 50%;
        position: absolute;
        bottom: -20px;

       
    }

    a::before{
        content: '';
        background-color: #3E86F3;
        bottom: -20px;
        left: 50%;
        transform: translateX(-50%);
        height: 0;
        width: 100%;
        z-index: 3;
        position: absolute;
        transition: all 400ms cubic-bezier(0.565, 0.020, 0.495, 0.990); /* custom */
        border-radius: 50%;
    }

    a:hover{
         &::after{
           height: 300%;
            border-radius: 50%;
        }
        &::before{
            height: 100%;
            bottom: 0;
            border-radius: 0;

        }
    }
</style>