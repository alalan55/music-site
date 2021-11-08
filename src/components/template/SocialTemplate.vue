<template>
    <div class="social">
       <div class="texts">
           <span class="title">SOCIAL</span>
             <span  class="sub-title">Me siga nas redes sociais</span>
       </div>
       <div class="icones">
           <div class="icon">
               <i class="fab fa-instagram"></i>
           </div>
           <div class="icon">
               <i class="fab fa-facebook"></i>
           </div>
            <div class="icon">
               <i class="fab fa-twitter"></i>
           </div>
       </div>

    </div>
</template>

<style lang="scss" scoped>
.social{
   max-width: 1300px;
  margin: 0 auto !important;
  padding: 4rem 0 !important;
   .texts {
    margin-bottom: 1.5rem !important;

    &>span{
        display: block;
        text-transform: uppercase;
    }
    .title {
      font-weight: 700;
      font-size: 1.7rem;
    }
    .sub-title{
        font-weight: 500;
    }
  }
  .icones{
      display: flex;
      flex-wrap: wrap;
        .icon{
            padding: 1rem !important;
            margin: .5rem !important;
            background: rgb(0, 0, 0);
            border-radius: 3px;
            cursor: pointer;
            transition: .1s ease-in;

            &:hover{
                background: rgb(49, 49, 49);
            }

            i{
                color: white;
            }
        }
  }
}

@media screen and (max-width: 600px){
    .social{
      padding: 1rem 1.5rem !important;
    }
}

</style>