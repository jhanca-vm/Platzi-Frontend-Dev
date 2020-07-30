<style>
  section {
    padding: 1rem;
    min-height: calc(100vh - 128px);
  }

  div {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    background-color: transparent;
    min-height: 530px;
  }

  h2 {
    text-align: center;
  }

  form {
    display: flex;
    flex-direction: column;
  }

  input {
    height: 50px;
    margin-bottom: 20px;
    padding: 0px 20px;
    font-size: 16px;
    border: none;
    border-bottom: 2px solid white;
    background-color: transparent;
  }

  input::placeholder {
    color: white;
  }

  button {
    height: 50px;
    margin: 10px 0px;
    font-size: 16px;
    font-weight: bold;
    letter-spacing: 1px;
    border-radius: 25px;
    background-color: rgba(255, 255, 255, 0.3);
    border: none;
    cursor: pointer;
  }

  a {
    text-align: center;
    color: #272343;
    opacity: 0.75;
  }

  a:hover {
    text-decoration: underline;
  }

  @media (min-width: 568px) {
    section {
      min-height: calc(100vh - 160px);
    }

    div {
      height: 580px;
      width: 400px;
      margin: 1rem auto;
      padding: 50px 50px 40px;
      border: 2px solid white;
      border-radius: 40px;
      background-color: rgba(255, 255, 255, 0.1);
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.25), 0 8px 10px rgba(0, 0, 0, 0.22);
    }
  }
</style>

<section>
  <div>
    <h2>Regístrate</h2>
    <form on:submit|preventDefault>
      <input type="text" placeholder="Nombre" />
      <input type="text" placeholder="Correo" />
      <input type="password" placeholder="Contraseña" />
      <button>Registrarme</button>
    </form>
    <a href="iniciar-sesion">Iniciar sesión</a>
  </div>
</section>
