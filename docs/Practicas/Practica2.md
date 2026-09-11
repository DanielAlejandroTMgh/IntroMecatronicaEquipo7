<html>
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>Temporizador 555</title>
	    <link rel="preconnect" href="https://fonts.googleapis.com"> <!-- Estas lineas de google fonts son para implementar fuentes de texto en la pagina web -->
	    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
	    <link href="https://fonts.googleapis.com/css2?family=Caacupe+One&family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&family=Passion+One:wght@400;700;900&display=swap" rel="stylesheet">
        <style type="text/css"> <!-- Estilos para la pagina-->
        h1{
            font-family: 'Passion One', sans-serif;
            font-size: 60px;
            text-align: left;
        }
        h2{
            font-family: 'Caacupe One', sans-serif;
            font-size: 30px;
            text-align: left;
        }
        p.texto{
            font-family: 'DM Sans', sans-serif;
            font-size: 12px;
            text-align: left;
        }
        </style>
    </head>
    <body markdown="1">
        <h1>MCU 101: ESP 32</h1>
        <p class="texto">El ESP 32 es un microcontrolador programable mediante un IDE que actúa como el cerebro de nuestro circuito para ejecutar las instrucciones especificadas por el código.</p>
        <h2>Blink</h2>
        <img src="../../recursos/imgs/WokwiEsquematico1.png" width="500" height="300">
        <img src="../../recursos/imgs/CodigoBlinkIDE.png">
        <h2>Blink con Botón</h2>
        <a href="../../recursos/videos/VideoBlinkboton.mp4">
            <img src="../../recursos/imgs/EsquematicoBlinkBoton.png" width="500" height="300">
        </a>
        <p>(hacer click en la imagen para el video)</p>
        <img src="../../recursos/imgs/CodigoBlinkbotonIDE.png">
        <h2>Bounce</h2>
       <a href="../../recursos/videos/VideoBounce.mp4">
            <img src="../../recursos/imgs/EsquematicoBlinkBoton.png" width="500" height="300"> <!-- Mismo esquematico -->
        </a>
        <p>(hacer click en la imagen para el video)</p>
        <img src="../../recursos/imgs/CodigoBounceIDE.png">
        <h2>¿Que es el Rebote de un Boton?</h2>
        <p class="texto">El rebote de un botón ocurre cuando presionamos el botón de 
        nuestro circuito , son como micro pulsaciones que detecta 
        aunque solo hayas presionado el botón una vez , no es 
        detectable ah simple vista , el rebote puede afectar un poco ya 
        que aunque nosotros no lo podemos ver el sistema si , lo que 
        ocasiona que interprete una pulsación como varias y en nuestro 
        circuito se apague y se prenda el led de manera muy rápida.</p>
        <h2>¿Por qué con INPUT_PULLUP la lógica queda invertida?</h2>
        <p class="texto">Cuando usamos INPUT_PULLUP en Arduino, la forma en que se 
        leen los valores del botón cambia un poco. Normalmente 
        cuando presionamos un botón obtenemos un 1 (HIGH) y 
        cuando no lo presionamos obtenemos un 0 (LOW). Pero 
        con INPUT_PULLUP pasa lo contrario. <br>
        Esto pasa porque Arduino utiliza una resistencia interna que 
        mantiene el pin en HIGH cuando el botón está sin presionar, 
        mientras no hacemos nada, Arduino está leyendo un 1, 
        entonces cuando presionamos el boton hace conexión con 
        GND (tierra) y al estar conectado a tierra el pin pasa a LOW , lo 
        que significa que es 0 y por lo tanto el Led se apaga.</p>
        <h2>Reporte de Fallas</h2>
        <p class="texto">En esta practica el unico erros que tuvimos fue que nos falto conectar un jumper y por lo tanto nuestro Led no prendia.
        Lo que hicimos para solucionarlo fue revisar que todo estuviera correctamente colocado y conectar el jumper que nos hacia falta</p>
    </body>
</html>