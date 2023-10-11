<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


Actividad: Adición de contenido multimedia en un sitio web utilizando etiquetas HTML5
Completa el siguiente código HTML añadiendo el contenido multimedia correspondiente en cada sección:

* 4 Imagenes.
* 2 Videos.
* 4 Audios.
* 2 Inline Frame.

Utiliza encabezados para títulos en cada elemento (<h1>...<h6>).

Crea una descripción para cada elemento utilizando párrafos (<p>).

Además, puedes emplear las siguientes etiquetas para mejorar la estructura y estilo de tu contenido:

Usa <strong> para resaltar texto importante.
Utiliza <br> para insertar saltos de línea si es necesario.
Agrega <span> para aplicar estilos específicos a porciones de texto.
Emplea <i> para enfatizar o dar énfasis a palabras o frases.
Utiliza <u> para subrayar texto cuando sea necesario.
Considera el uso de <div> para crear secciones o contenedores para tu contenido, lo que puede facilitar la organización y el diseño de la página.

### Solución.

<!DOCTYPE html>
<html>

<head>
    <title>Etiquetas Multimedia HTML5</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }

        header {
            background-color: #2d9ada;
            color: white;
            padding: 20px;
            text-align: center;
        }

        section {
            border: 1px solid #ddd;
            padding: 20px;
            margin-bottom: 20px;
        }

        h2 {
            color: rgb(21, 21, 27);
        }

        footer {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>

<body>

    <header>
        <h1>TROPIVUELTAS</h1>
        <h3>Servicio de Mensajeria, diligencias, consignaciones y mas</h3>
    </header>

    <section>

        <h1>Que es la Mensajeria?</h1>


        <p>Es el servicio de transporte y reparto de cartas y paquetes, generalmente dentro de una misma población....
            <a href="https://www.google.com/search?q=que+es+la+mensajeria&rlz=1C1CHBF_esCO1003CO1003&oq=que+es+la+mensajeria&gs_lcrp=EgZjaHJvbWUyCQgAEAAYQxiKBTIGCAEQRRg5MgcIAhAAGIAEMgcIAxAAGIAEMgwIBBAAGBQYhwIYgAQyBwgFEAAYgAQyBwgGEAAYgAQyBwgHEAAYgAQyBwgIEAAYgAQyBwgJEAAYgATSAQg2MjEzajBqN6gCALACAA&sourceid=chrome&ie=UTF-8"
                target="_blank">mas informacion</a>
        </p>
        <br>
        <br>
        <br>


        <img src="mensajero.jpg" alt="mensajero" width="300">


        <h1>Quien invento la mensajeria?</h1>


        <p>Jenofonte atribuyó el primer uso de los mensajeros al príncipe Persa, Se dice que el mensajero de la griego
            antiguo corrió 26 millas desde Maratón hasta Atenas para llevar la noticia de la victoria griega sobre los
            persas en el año 490 a. C. La carrera de larga distancia conocida como maratón debe su nombre a esta
            carrera..
            <a href="https://es.wikipedia.org/wiki/Mensajero#:~:text=Jenofonte%20atribuy%C3%B3%20el%20primer%20uso,C."
                target="_blank">mas informacion</a>
        </p>
        <br>
        <br>
        <br>


        <img src="mensajero antiguo.jpg" alt="mensajero antiguo" width="300">


        <h1>Por que es importante la mensajeria de productos?</h1>

        <p>La entrega oportuna y segura de los productos y documentos es esencial para generar confianza entre las
            empresas y sus clientes. La mensajería y la paquetería confiables y eficientes demuestran el compromiso de
            una empresa con la excelencia en el servicio al cliente y la calidad de sus productos.
            <a href="https://mundoautonomos.org/importancia-mensajeria-paqueteria-en-las-empresas/#:~:text=La%20entrega%20oportuna%20y%20segura,la%20calidad%20de%20sus%20productos."
                target="_blank">mas informacion</a>
        </p>
        <br>
        <br>
        <br>


        <img src="importancia de mensajero.jpg" alt="importancia de mensajero" width="400">
    </section>


    <h1>Que ofrece un servicio de mensajeria?</h1> <!-- Esta pagina de internet esta creada para solucionar tareas que en el momento la gente no pueda realizar -->


    <p>Los servicios que prestan estas empresas de mensajería incluyen la recogida, admisión, clasificación, transporte,
        distribución y entrega de cualquier carta o paquete, así como el envío de giros postales (envío de dinero a un
        destinatario).
        <a href="https://www.google.com/search?q=la+mensajeria+de+productos&sca_esv=557962971&rlz=1C1CHBF_esCO1003CO1003&sxsrf=AB5stBh3GcEPeKlr-r433rB98UEWMbhwqQ%3A1692321224469&ei=yMXeZNb4G_OuqtsPsN-fuAU&ved=0ahUKEwjW_Lfrg-WAAxVzl2oFHbDvB1cQ4dUDCA8&uact=5&oq=la+mensajeria+de+productos&gs_lp=Egxnd3Mtd2l6LXNlcnAiGmxhIG1lbnNhamVyaWEgZGUgcHJvZHVjdG9zMgUQABiiBDIFEAAYogQyBRAAGKIESNXAAVDyGFjuuQFwDngBkAEAmAGfAqABkUeqAQcwLjIwLjI0uAEDyAEA-AEBqAIUwgIKEAAYRxjWBBiwA8ICBxAjGOoCGCfCAhYQABgDGI8BGOoCGLQCGIwDGOUC2AEBwgIWEC4YAxiPARjqAhi0AhiMAxjlAtgBAcICBRAAGIAEwgILEAAYgAQYsQMYgwHCAhEQLhiABBixAxiDARjHARjRA8ICCxAAGIoFGLEDGIMBwgILEC4YgAQYxwEYrwHCAgsQLhiKBRixAxiDAcICCBAAGIAEGLEDwgIHEAAYigUYQ8ICDhAuGIAEGLEDGMcBGK8BwgIFEC4YgATCAgsQLhiABBixAxiDAcICDhAAGIAEGLEDGIMBGMkDwgIIEAAYigUYkgPCAg0QLhiKBRixAxiDARhDwgIIEC4YgAQYsQPCAhcQLhiABBixAxiXBRjcBBjeBBjgBNgBAsICDRAuGA0YgAQYsQMYsQPCAgcQABgNGIAEwgIZEC4YDRiABBixAxiXBRjcBBjeBBjgBNgBAsICBxAhGKABGArCAgsQLhiDARixAxiABMICChAAGIAEGBQYhwLCAhQQLhiABBiXBRjcBBjeBBjgBNgBAsICBxAuGA0YgATCAhYQLhgNGIAEGJcFGNwEGN4EGOAE2AECwgIGEAAYHhgNwgIIEAAYHhgNGA_CAggQABgIGB4YDcICDxAAGAgYHhgNGA8Y8QQYCsICCBAAGBYYHhgPwgIGEAAYFhgewgIFECEYoAHiAwQYACBBiAYBkAYIugYGCAEQARgLugYGCAIQARgU&sclient=gws-wiz-serp"
            target="_blank">mas informacion</a>
    </p>
    <br>
    <br>
    <br>


    <img src="servicio de mensajeria.jpg" alt="Servicio de mensajeria" width="400"> </section>


    <section>
        <h2>Videos</h2>
        <p> <strong>DOMICILIO GRATIS AREA METROPOLITANA....!</strong></p>
        <br>
        <br>

        <video src="Domicilio gratis.mp4" controls width="400"></video>
        
        
        <h2>Videos</h2>
        <p>Aqui encontraras la recepcion de mercancia de los productos para su pronta entrega.</p>
        <br>
        <br>

        <video src="mercancia.mp4" controls width="250"></video>


        <h2>Videos</h2>
        <p>Aqui encontraras el transporte de sus productos.</p>
        <br>
        <br>

        <video src="mensajero moto.mp4" controls width="400"></video>
        
        
        <h2>Videos</h2>
        <p>Aqui te mostramos el proceso de nuestros servicios.</p>
        <br>
        <br>

        <video src="Diligencias moto.mp4" controls width="400"></video>
    </section>

   
    <section>
        <h2>Bienvenida</h2>
        <p>Bienvenidos a <strong>TROPIVUELTAS</strong> Servicio de Mensajeria, diligencias, consignaciones y mas; Contamos con la mejor logistica personalizada para que tus tareas o envios se realicen de forma rapida y agil.</p>

        <audio src="tension.mp3" controls></audio>
        
        
        <h2>Contáctanos</h2>
        <p>Este es el primer paso para el inicio de muchas entregas y emociones que vamos a tener juntos,
            muchas gracias por confiar en nosotros, en un momento nos comunicaremos contigo.</p>

        <audio src="chatea con nosotros.mp3" controls></audio>
        
        
        <h2>Recogida y entrega</h2>
        <p>Te cuidamos tus envios como si fueran nuestros; no te preocupes que estan en buenas manos.</p>

        <audio src="Recogida y entrega.mp3" controls></audio>
        
        
        <h2>Llegada del mensajero</h2>
        <p>Te hacemos la entrega en el lugar que tu elijas a la hora que decidas, recuerda que tu tranquilidad es la nuestra.
            <strong>De nuevo GRACIAS por confiar en nosotros!.</strong></p>

        <audio src="llegada del mensajero.mp3" controls></audio>
        
        
    </section>

    <section>
        <h2>Mensajeria</h2>
        <p>Lo que debes saber de un mensajero...</p>
        <iframe width="560" height="315" src="https://www.educaweb.com/profesion/mensajero-moto-654/#:~:text=Los%20mensajeros%20en%20moto%20transportan,y%20garantizan%20su%20entrega%20segura." frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </section>

        <h2>Manual de mensajeria</h2>
        <p>Todo lo que debes saber para ser un buen mensajero...</p>
        <iframe width="560" height="315" src="https://serwell.es/que-es-motomensajeria/" frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </section>

    <footer>
        <p><i><strong>Fernando Sánchez Arenas</strong></i></p> <!-- Futuro programador con ayuda de Dios -->
        <br>
        <br>
        CESDE
        <br>
        <br>
        &copy;2023
    </footer>

</body>

</html>

### Link de la pagina

file:///C:/Users/Fidel/OneDrive/Documentos/PAGINA%20WEB%20TROPIVUELTAS/Index.html




             





