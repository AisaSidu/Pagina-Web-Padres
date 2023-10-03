<html>
<head>
    <title style="font-size: 24px; font-family: 'Lexend', cursive;">Isaak Vidal</title>
    <style>
        body {
            background-color: #1465bb;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
            height: 100vh;
            margin: 0;
            font-family: 'Lexend', cursive;
        }
        h1 {
            font-family: 'Lexend', cursive;
            color: white;
            margin-top: 20px;
        }
        p {
            font-size: 18px;
            color: white;
        }
        /* Estilo para los botones */
        .boton {
            width: 150px;
            height: 50px;
            background-color: #007bff;
            border: 2px solid #007bff;
            border-radius: 10px;
            padding: 10px;
            cursor: pointer;
            color: white;
            font-weight: bold;
            margin: 10px;
        }
        .boton:hover {
            background-color: #0056b3;
        }
        /* Estilo para el contenido */
        #contenido {
            max-width: 800px;
            margin: 0 auto;
            padding: 10px;
            border: 1px solid #ccc;
            background-color: white;
        }
        /* Estilo para las imágenes dentro del contenido */
        #contenido img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
        }
        /* Oculta el contenido por defecto */
        #mama, #papa {
            display: none;
        }
    </style>
</head>
<body>
	<center>
    <h1>Bienvenido</h1>
	</center>

    <!-- Texto de introducción -->
    <p>¡Hola! Mi nombre es Isaak Vidal y esta página es un tributo a mis padres.</p>

<center>
<img src="Uhme.jpg" alt="Descripción de la imagen" width="280" height="300" style="border-radius: 50%;" ><Br><Br>
</center>


    <!-- Contenedor para el texto con márgenes laterales y borde -->
    <div style="max-width: 800px; margin: 0 auto; padding: 10px; border: 1px solid #ccc;">
        <!-- Texto -->
        <p>Este soy yo, nací el 16 de diciembre del 2002 en Estados Unidos, Indiana. Mis padres son Armando Vidal y Normallín García, siendo yo su primer hijo y hermano mayor de mis hermanos, actualmente soy estudiante de universidad y me gusta mucho el pan.</p>
    </div>
	<center>
    <!-- Botón para Mamá -->
    <div class="boton" onclick="mostrarContenido('mama')">Mamá</div>
    	</center>
	<center>
    <!-- Botón para Papá -->
    <div class="boton" onclick="mostrarContenido('papa')">Papá</div>
    	</center>

    <!-- Contenido para Mamá -->
	<center>
    <div id="mama">
        <h2>Mi Mamá</h2>
        <p>Mi mamá, Normallin Garcia, es alguien a quien he admirado mucho en todo aspecto, es quien ha estado conmigo desde toda la vida para apoyarme en mis metas. Su personalidad es muy seria y callada, pero definitivamente es afectiva a su manera. Me encanta su persecipción positiva y lógica de ver las cosas, también siempre ha sido muy comprensiva conmigo y mis hermanos en todo aspecto, por lo que siempre nos hemos sentido apoyados por ella. <Br><Br>

Actualmente tiene 45 años y admiro todo el esfuerzo que hace, se encarga de la casa, además de cuidar niños y a mi hermano más pequeño al mismo tiempo, definitivamente una persona trabajadora de quien tengo mucho que aprender. <Br>




</p>
	<center>
        <img src="mom.jpg" alt="Imagen de Mamá" width="280" height="300" style="border-radius: 50%;" >
	</center>
    </div>

    <!-- Contenido para Papá -->
	<center>
    <div id="papa">
        <h2>Mi Papá</h2>
        <p>Mi papá, Armando Vidal es una persona muy trabajadora, de caracter fuerte y definitivamente es un buen lider. Desde que tengo memoria lo he recordado como una persona muy grande y estricta. <Br>
A pesar de todo lo anterior, también es muy cariñoso y gracioso y trata de hallar formas de acercarse a mí y a mis hermanos. Definitivamente una persona grandiosa de la cual estoy orgulloso, una persona la cual sabe como resolver las cosas en cualquier situación. <Br><Br>

Actualmente tiene 42 años y trabaja como supervisor. <Br>
</p>
	<center>
        <img src="dad.jpg" alt="Imagen de Papá" width="280" height="300" style="border-radius: 50%;" > 
	</center>
    </div>

    <!-- JavaScript para mostrar/ocultar el contenido -->
    <script>
        function mostrarContenido(idContenido) {
            var contenido = document.getElementById(idContenido);
            var contenidoAnterior = document.querySelector("#contenido > div:not(#" + idContenido + ")");
            if (contenido.style.display === "none" || contenido.style.display === "") {
                contenido.style.display = "block";
                contenidoAnterior.style.display = "none";
            } else {
                contenido.style.display = "none";
            }
        }
    </script>

