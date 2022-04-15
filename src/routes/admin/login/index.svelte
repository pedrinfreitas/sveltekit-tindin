<svelte:head>
  <title>Login - Tindin</title>
</svelte:head>

<section class="page__login">
  <div class="login__card">
    <img
      src="/logo_tindin_120x120px.webp"
      alt="logo Tindin"
      width="72"
      height="62"
    />

    <div>
      <label for="email"> E-mail </label>
      <input id="email" type="text" placeholder="usuario@email.com" />
    </div>

    <div>
      <label for="password"> Senha </label>
      <input id="password" type="password" placeholder="Digite sua senha" />
    </div>

    <button>ACESSAR</button>
    <a href="/admin/login/recover-password">Esqueci minha senha</a>
    <a href="/admin/register">Quero me registrar</a>
  </div>
</section>

<style lang="scss">
  .page__login {
    height: 100vh;
    background-color: #b8306d;
    display: grid;
    place-items: center;
    .login__card {
      display: flex;
      flex-direction: column;
      align-items: center;
      background-color: white;

      img {
        margin: 3rem 0 3rem;
      }

      div {
        display: flex;
        flex-direction: column;
        width: 100%;

        label {
          color: #1736b3;
          z-index: 1;
          margin: 1rem 1.5rem;
          padding: 0 0.25rem;
          margin-bottom: -0.5rem;
          background: white;
          width: 5ch;
          font-family: "Inter", sans-serif;
          font-weight: 500;
          font-size: 12px;
        }
        input {
          margin: 0 1rem;
          padding: 0 0.5rem;
          height: 3.5rem;
          border: 2px solid #d7d3d3;
          border-radius: 4px;
          font-weight: 400;
          font-size: 1rem;
        }
      }

      button {
        color: white;
        background-color: #b8306d;
        margin: 2rem 1rem;
        border: none;
        border-radius: 20px;
        width: calc(100% - 2rem);
        height: 3.25rem;
        padding: 0.5rem;
        font-weight: 700;
        font-size: 14px;
      }

      a {
        font-weight: 600;
        font-size: 1.25rem;
        margin-bottom: 2rem;
      }
    }
  }

  @media screen and (min-width: 480px) {
    .page__login {
      .login__card {
        background-color: white;
        border-radius: 2rem;
        width: 400px;
      }
    }
  }
  @media screen and (max-width: 480px) {
    .login__card {
      width: 100vw;
      height: 100vh;
      border-radius: 0;
    }
  }
</style>
