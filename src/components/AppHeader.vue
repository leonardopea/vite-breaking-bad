<script>
export default {
    
}
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col">
                <button class="button_circle_big"></button>
            </div>
            <div class="col">
                <button class="button_circle_small"></button>
                <button class="button_circle_small_due"></button>
                <button class="button_circle_small_tre"></button>
            </div>
        </div>
    </div>

</template>


<style lang="scss" scoped>

@use '../styles/partials/mixsins' as *;

    .container{
        max-width: 1180px;
        background-color: #B71B1B;
        margin-top: 50px;


        .row{
            display: flex;

            .col{
                padding: 20px
            }


        }

    }



    .button_circle_big{
        @include bottone_circolare;
        @include bottone_grande;
        background: rgb(2,0,36);
        background: linear-gradient(332deg, rgba(2,0,36,1) 0%, rgba(9,9,121,1) 30%, rgba(255,255,255,1) 100%); 
    }

    .button_circle_small{
        @include bottone_circolare;
        @include bottone_piccolo;
        background: rgb(255,212,212);
        background: linear-gradient(90deg, rgba(255,212,212,1) 0%, rgba(255,140,140,1) 30%, rgba(255,55,55,1) 100%); 
        

    }

    .button_circle_small_due{
        @include bottone_circolare;
        @include bottone_piccolo;
        background: rgb(255,212,212);
        background: linear-gradient(90deg, rgba(252,252,197,1) 0%, rgba(255,255,136,1) 30%, rgba(255,255,56,1) 100%); 
        margin-left: 15px

    }

    .button_circle_small_tre{
        @include bottone_circolare;
        @include bottone_piccolo;
        background: rgb(217,236,217);
        background: linear-gradient(90deg, rgba(217,236,217,1) 0%, rgba(148,202,148,1) 30%, rgba(58,157,58,1) 100%);
        margin-left: 15px 

    }
</style>