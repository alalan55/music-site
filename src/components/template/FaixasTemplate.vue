<template>
  <div class="faixas">
    <div class="title">
      <span>ALGUMAS FAIXAS PRESENTES NO ALBUM</span>
    </div>

    <div class="lps">
      <div class="lp one">
        <div class="img"></div>
        <div class="descricoes">
          <div class="title">
            <span>EP</span>
          </div>
          <div class="name">
            <span>Saturno</span>
          </div>
        </div>
      </div>
      <div class="lp two">
        <div class="img"></div>
        <div class="descricoes">
          <div class="title">
            <span>EP</span>
          </div>
          <div class="name">
            <span>Lifes</span>
          </div>
        </div>
      </div>
      <div class="lp trhee">
        <div class="img"></div>
        <div class="descricoes">
          <div class="title">
            <span>EP</span>
          </div>
          <div class="name">
            <span>Cosmos</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.faixas {
  height: auto;
  max-width: 1300px; //verificar melhor esse cara aquiiiii
  margin: 0 auto !important;
  padding: 4rem 0 !important;


  .title {
    margin-bottom: 1.5rem !important;
    span {
      font-weight: 700;
      font-size: 1.7rem;
    }
  }

  .lps {
    // border: 1px solid red;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: space-between;


    .lp {
      flex: 1 1 300px;
      .img {
        height: 50vh;
        width: 50vh;
        transition: transform .2s ;
        overflow: hidden !important;

        &:hover{
           // transform: scale(1.1);
        }
      }
      .descricoes {
        margin: 2rem 0 !important;
        .title {
          font-weight: 700;
          font-size: 1.4rem;
          margin: 0.5rem 0 !important;
        }
        .name {
          font-size: 1.5rem;
          font-weight: 500;
        }
      }
    }

    .one {
      .img {
        background: url(https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=288,h=304,fit=crop/A3QN2R7yxgHkQNM4/releases-c-AzGRJlDL6xiD74Z2.webp)
          no-repeat;
        background-size: cover;
        background-position: center;
      }
    }
    .two {
      .img {
        background: url(https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=288,h=304,fit=crop/A3QN2R7yxgHkQNM4/releases-c-AVLnvRNjZMfVel84.webp)
          no-repeat;
        background-size: cover;
        background-position: center;
      }
    }
    .trhee {
      .img {
        background: url(https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=288,h=304,fit=crop/A3QN2R7yxgHkQNM4/releases-c-A1aynMrx4yiGkRnP.webp)
          no-repeat;
        background-size: cover;
        background-position: center;
      }
    }
  }
}
@media screen and (max-width: 1350px) {
  .lps {
    .lp {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
    }
  }
}

@media screen and (max-width: 650px){
  .faixas{
    text-align: center;
    padding: 0 1.5rem !important;
    .title span{
      font-size: 1.3rem !important;
    }
  }

  .lp{
    .img{
      width: 100% !important;
    }
  }
}
</style>