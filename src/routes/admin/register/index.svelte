<div class="page">
  <img
    src="/logo_tindin_120x120px.webp"
    alt="logo Tindin"
    width="72"
    height="62"
  />
  <div class="box__card">
    <a href="/admin/register/student">
      <div class="box__card--student">
        <img src="/images/student.svg" alt="" width="172" height="182" />
        <p>ALUNO</p>
      </div>
    </a>

    <a href="/admin/register/teacher">
      <div class="box__card--teacher">
        <img src="/images/teacher.svg" alt="" width="172" height="182" />
        <p>PROFESSOR</p>
      </div>
    </a>
  </div>

  <a href="/admin/login">Sou tutor legal ou autorizado</a>
  <a href="/admin/login">voltar</a>
</div>

<style lang="scss">
  .page {
    display: flex;
    flex-direction: column;
    align-items: center;

    > img {
      margin: 3rem 0 1rem;
    }

    .box__card {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;

      a {
        text-decoration: none;
        &:visited {
          color: white;
        }
      }
      div {
        padding: 1rem;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-evenly;

        min-width: 320px;
        min-height: 320px;
        color: white;
        font-size: 34px;
        text-align: center;
        border-radius: 20px;
        margin: 0 1rem 1rem;
      }

      &--student {
        background: #ed9d47;
      }

      &--teacher {
        background: #4769ed;
      }
    }
  }

  @media screen and (min-width: 321px) and (max-width: 768px) {
    .page {
      .box__card {
        div {
          font-size: 24px;
          min-width: 280px;
          min-height: 200px;
        }
      }
    }
  }
  @media screen and (max-width: 320px) {
    .page {
      .box__card {
        div {
          font-size: 24px;
          min-width: 240px;
          min-height: 140px;
          img {
            width: 33%;
          }
        }
      }
    }
  }
</style>
