<!DOCTYPE html>

<html lang="es">

<head>

  <base target="_top">

  <meta charset="UTF-8">

  <meta
    name="viewport"
    content="width=device-width, initial-scale=1.0"
  >

  <title>Formulario de contacto</title>


  <style>

    * {
      box-sizing: border-box;
    }


    body {

      margin: 0;

      min-height: 100vh;

      font-family:
        Arial,
        Helvetica,
        sans-serif;

      background:
        linear-gradient(
          135deg,
          #eef2f6,
          #dce2e8
        );

      display: flex;

      align-items: center;

      justify-content: center;

      padding: 20px;

      color: #1f2937;

    }


    .contenedor {

      width: 100%;

      max-width: 430px;

      background: #ffffff;

      border-radius: 16px;

      padding: 32px;

      box-shadow:
        0 10px 35px
        rgba(0, 0, 0, 0.12);

    }


    .icono {

      width: 58px;

      height: 58px;

      margin:
        0 auto 18px;

      border-radius: 50%;

      background: #2563eb;

      color: #ffffff;

      display: flex;

      align-items: center;

      justify-content: center;

      font-size: 24px;

      font-weight: bold;

    }


    h1 {

      margin: 0 0 10px;

      text-align: center;

      font-size: 26px;

      color: #111827;

    }


    .descripcion {

      margin:
        0 0 28px;

      text-align: center;

      color: #6b7280;

      font-size: 15px;

      line-height: 1.5;

    }


    .grupo {

      margin-bottom: 18px;

    }


    label {

      display: block;

      margin-bottom: 7px;

      font-size: 14px;

      font-weight: bold;

      color: #374151;

    }


    input {

      width: 100%;

      height: 48px;

      padding: 0 14px;

      border:
        1px solid #d1d5db;

      border-radius: 9px;

      background: #ffffff;

      color: #111827;

      font-size: 16px;

      outline: none;

    }


    input:focus {

      border-color: #2563eb;

      box-shadow:
        0 0 0 3px
        rgba(37, 99, 235, 0.12);

    }


    button {

      width: 100%;

      height: 50px;

      border: none;

      border-radius: 9px;

      background: #2563eb;

      color: #ffffff;

      font-size: 16px;

      font-weight: bold;

      cursor: pointer;

    }


    button:hover {

      background: #1d4ed8;

    }


    button:disabled {

      background: #9ca3af;

      cursor: not-allowed;

    }


    .mensaje {

      display: none;

      margin-top: 18px;

      padding: 13px;

      border-radius: 9px;

      text-align: center;

      font-size: 14px;

      line-height: 1.4;

    }


    .mensaje.enviando {

      display: block;

      background: #eff6ff;

      color: #1d4ed8;

    }


    .mensaje.correcto {

      display: block;

      background: #ecfdf5;

      color: #047857;

    }


    .mensaje.error {

      display: block;

      background: #fef2f2;

      color: #b91c1c;

    }


    .informacion {

      margin-top: 20px;

      padding: 13px;

      border-radius: 9px;

      background: #f3f4f6;

      color: #6b7280;

      font-size: 12px;

      line-height: 1.5;

      text-align: center;

    }


    .pie {

      margin-top: 22px;

      text-align: center;

      color: #9ca3af;

      font-size: 11px;

    }


  </style>

</head>


<body>


  <div class="contenedor">


    <div class="icono">
      C
    </div>


    <h1>
      Formulario de contacto
    </h1>


    <p class="descripcion">
      Completa tus datos para enviar tu solicitud.
    </p>


    <form id="formulario">


      <div class="grupo">

        <label for="nombre">
          Nombre
        </label>

        <input
          type="text"
          id="nombre"
          name="nombre"
          placeholder="Escribe tu nombre"
          autocomplete="given-name"
          maxlength="100"
          required
        >

      </div>


      <div class="grupo">

        <label for="apellidos">
          Apellidos
        </label>

        <input
          type="text"
          id="apellidos"
          name="apellidos"
          placeholder="Escribe tus apellidos"
          autocomplete="family-name"
          maxlength="150"
          required
        >

      </div>


      <button
        type="submit"
        id="botonEnviar"
      >
        Enviar datos
      </button>


    </form>


    <div
      id="mensaje"
      class="mensaje"
    ></div>


    <div class="informacion">

      Los datos introducidos se utilizarán
      únicamente para gestionar esta solicitud
      y contactar contigo cuando sea necesario.

    </div>


    <div class="pie">

      Formulario de contacto

    </div>


  </div>


  <script>


    const formulario =
      document.getElementById("formulario");


    const nombre =
      document.getElementById("nombre");


    const apellidos =
      document.getElementById("apellidos");


    const botonEnviar =
      document.getElementById("botonEnviar");


    const mensaje =
      document.getElementById("mensaje");


    formulario.addEventListener(
      "submit",
      function(event) {

        event.preventDefault();


        const nombreValor =
          nombre.value.trim();


        const apellidosValor =
          apellidos.value.trim();


        if (
          !nombreValor ||
          !apellidosValor
        ) {

          mostrarError(
            "Debes completar los dos campos."
          );

          return;

        }


        botonEnviar.disabled = true;

        botonEnviar.textContent =
          "Enviando...";


        mensaje.className =
          "mensaje enviando";

        mensaje.textContent =
          "Enviando tus datos...";


        google.script.run

          .withSuccessHandler(
            function(respuesta) {

              if (
                respuesta &&
                respuesta.ok
              ) {

                mensaje.className =
                  "mensaje correcto";

                mensaje.textContent =
                  respuesta.mensaje;

                formulario.reset();

              } else {

                mostrarError(
                  respuesta &&
                  respuesta.mensaje
                    ? respuesta.mensaje
                    : "No se pudieron enviar los datos."
                );

              }


              botonEnviar.disabled = false;

              botonEnviar.textContent =
                "Enviar datos";

            }
          )

          .withFailureHandler(
            function(error) {

              mostrarError(
                error &&
                error.message
                  ? error.message
                  : "Se produjo un error al enviar los datos."
              );


              botonEnviar.disabled = false;

              botonEnviar.textContent =
                "Enviar datos";

            }
          )

          .enviarDatos(
            nombreValor,
            apellidosValor
          );

      }
    );


    function mostrarError(texto) {

      mensaje.className =
        "mensaje error";

      mensaje.textContent =
        texto;

    }


  </script>


</body>

</html>
