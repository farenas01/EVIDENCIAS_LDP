<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 9 


### Solución

### Actividad: Propiedades de espaciado y unidades de medida

Objetivo:


Practicar el uso de las propiedades de espaciado margin, padding, border y border-radius, con diferentes unidades de medida.

Crea un nuevo archivo HTML y CSS.
En el archivo HTML, agrega el siguiente código:

<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Propiedades de espaciado</title>
  <link rel="stylesheet" href="style.css">
</head>
<body> 
  <div class="contenedor">
    <div class="elemento"></div>
  </div>
</body>
</html>

## Preguntas:

1. ¿Qué es la propiedad margin?

#### Respuesta

* Margin: Agrega un margen de 10 píxeles a todos los lados del elemento.

##### Ejemplo:
  
    .elemento {
      margin: 10px;
      width: 100px;
      height: 100px;
    }

2. ¿Qué es la propiedad padding?

#### Respuesta

* Padding: Agrega un relleno de 20 píxeles a todos los lados del elemento.

##### Ejemplo:

    .elemento {
      padding: 20px;
      margin: 10px;
      width: 100px;
      height: 100px;
    }

3. ¿Qué es la propiedad border?

#### Respuesta

* Border: Agrega un borde de 5 píxeles de color rojo.

##### Ejemplo: 

    .elemento {
      border: 5px solid red;
      padding: 20px;
      margin: 10px;
      width: 100px;
      height: 100px;
    }


4. ¿Qué es la propiedad border-radius?

#### Respuesta

* Border-radius: Agrega un radio de esquina de 10 píxeles.

##### Ejemplo: 

    .elemento {
      border-radius: 10px;
      border: 5px solid red;
      padding: 20px;
      margin: 10px;
      width: 100px;
      height: 100px;
    }


5. ¿Qué unidades de medida se pueden utilizar para las propiedades de espaciado?

#### Respuesta

* Unidades de medida: Prueba diferentes unidades de medida para las propiedades de espaciado. Por ejemplo, puedes usar unidades porcentuales (%) para establecer un margen o relleno del 50%.

##### Ejemplo:

    .elemento {
      border-radius: 10px;
      border: 5px solid red;
      margin: 50%;
      padding: 50%;
      width: 100px;
      height: 100px;
    }








