<template>
  <div class="capa">
    <div class="content">
      <div class="lado-direito"></div>
      <div class="lado-esquerdo">
        <div class="textos">
          <div class="description">
            <span
              >Feel what you <br />
              haven't felt</span
            >
          </div>

          <div class="name">
            <h1>
              DON <br />
              donno
            </h1>
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
.capa {
  // background: url(https://images.pexels.com/photos/3320136/pexels-photo-3320136.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260) no-repeat;
  background: url(https://images.pexels.com/photos/1550469/pexels-photo-1550469.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260)
    no-repeat;
  background-size: cover;
  height: 100vh;
  width: 100%;
  background-position: center;

  .content {
    display: flex;
    flex-wrap: wrap;
    height: 100%;
    width: 100%;

    & > div {
      flex: 1 1 300px;
    }

    .lado-esquerdo {
      text-transform: uppercase;
      display: flex;
      align-items: center;
      color: white;
      align-items: flex-end;

      .textos {
        padding-bottom: 5rem !important;
        .description {
          span {
            font-weight: 500;
            font-size: 1.5rem;
          }
        }

        .name {
          h1 {
            font-weight: 800;
            font-size: 7rem;
            transition: .2s ease-in-out;
          }
        }
      }
    }
  }
}


@media screen and (max-width: 700px){
    .textos {

        .name {
          h1 {
            font-weight: 700;
            font-size: 4rem !important;
          }
        }
      }

}
</style>