<template>
  <div class="sobre">
    <div class="title">
      <span>Quem sou eu?</span>
    </div>

    <div class="descricao">
      <p>
          Quasi vitae unde esse neque eos culpa commodi
        voluptas illum autem quia expedita, blanditiis ipsa laboriosam corporis
        voluptatum eius.
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laudantium,
        consequatur optio. Quasi vitae unde esse neque eos culpa commodi
        voluptas illum autem quia expedita, blanditiis ipsa laboriosam corporis
        voluptatum eius.
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.sobre {
 height: auto;
  max-width: 1300px; //verificar melhor esse cara aquiiiii
  margin: 0 auto !important;
  padding: 4rem 0 !important;

  .title {
    margin-bottom: 1.5rem !important;
    span {
      font-weight: 700;
      font-size: 1.7rem;
      text-transform: uppercase;
    }
  }
  .descricao{
      p{
          font-size: 1.2rem
      }
  }
}

@media screen and (max-width: 600px){
    .sobre{
      padding: 1rem 1.5rem !important;
      margin-top: 1rem !important;
    }
}
</style>