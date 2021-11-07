<template>
    <div class="background">
        <div class="descricao">
            <span>FELL THE MOVIMENT</span>
        </div>

    </div>
</template>

<style lang="scss" scoped>
.background{
    width: 100%;
    height: 40vh;
    background:  url(https://images.pexels.com/photos/3742711/pexels-photo-3742711.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260) no-repeat;
    background-size: cover;
    background-attachment: fixed;

    .descricao{
        width: 100%;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;

        span{
            font-size: 3rem;
            font-weight: 600;
            color: white;
            transition: .2s ease-in-out;
        }
    }
}

@media screen and (max-width:600px){
    .descricao{
        // display: none !important;
        span{
            font-size: 1rem !important;
        }
    }
}

</style>