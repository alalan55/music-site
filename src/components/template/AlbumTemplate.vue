<template>
  <div class="album">
    <div class="content-album">
      <div class="imagem-algum">
        <div class="img"></div>
      </div>
      <div class="lancamento">
        <div class="descriptions">
          <div class="release">
            <div class="new">
              <span>NOVO LANÇAMENTO 01/12/21</span>
            </div>

            <div class="album-lancamento">
              <span
                >REQUEST <br />
                (ALBUM)</span
              >
            </div>
          </div>

          <div class="disponivel">
            <span class="title"> DISPONÍVEL EM:</span>
            <div class="icons">
              <div class="icon">
                <i class="fab fa-spotify"></i>
              </div>
              <div class="icon">
                <i class="fab fa-apple"></i>
              </div>

              <div class="icon">
                <i class="fab fa-deezer"></i>
              </div>

              <div class="icon">
                <i class="fab fa-youtube"></i>
              </div>
            </div>
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
.album {
  height: 100vh;
  max-width: 1500px;
  margin: 0 auto !important;
  padding: 4rem 0 !important;

  .content-album {
    height: 100%;

    display: flex;
    flex-wrap: wrap;

    & > div {
      flex: 1 1 600px;
    }

    .imagem-algum {
      display: flex;
      align-items: center;
      justify-content: center;
      .img {
        height: 70vh;
        width: 70vh;
        background: url(https://images.pexels.com/photos/209831/pexels-photo-209831.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260)
          no-repeat;
        background-size: cover;
        background-position: center;
      }
    }
    .lancamento {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;

      .descriptions {
        height: 70vh;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;

        .new {
          margin: 0.5rem 0 !important;
          span {
            font-weight: 500;
          }
        }

        .album-lancamento {
          margin: 0.5rem 0 !important;
          span {
            font-weight: 800;
            font-size: 3rem;
          }
        }
      }

      .disponivel {
        .title {
          font-size: 1.3rem;
          font-weight: 800;
        }

        .icons {
          display: flex;

          .icon {
            padding-top: 1rem !important;
            margin: 0 2rem 0 0 !important;

            i {
              font-size: 1.5rem;
              cursor: pointer;
              transition: 0.2s ease-in-out;

              &:hover {
                color: rgb(37, 37, 37);
              }
            }
          }
        }
      }
    }
  }
}

@media screen and (max-width: 1250px) {
  .album {
    height: auto !important;
  }
  .lancamento {
      .descriptions {
        text-align: center !important;
        .disponivel {
          .icons {
            align-items: center;
            justify-content: center;
          }
        }
      }
    }
}

@media screen and (max-width: 1024px) {
  .content-album {
    .imagem-algum {
      .img {
        width: 50vh !important;
        height: 50vh !important;
      }
    }

    .lancamento {
      height: 35vh;
      .descriptions {
        text-align: center !important;
        .disponivel {
          .title{
            font-size: 1rem !important;
          }
          .icons {
            align-items: center;
            justify-content: center;
          }
        }
        .album-lancamento{
          span{
            font-size: 1.5rem !important;
          }
        }
      }
    }
  }
}
</style>