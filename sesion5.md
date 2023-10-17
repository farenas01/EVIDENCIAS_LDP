<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


Actividad: Diseñar un formulario de pedido de un producto
Objetivo:

Aplicar los conocimientos sobre los tipos de etiquetas HTML para diseñar un formulario de pedido de un producto.

Instrucciones:

Crear un nuevo documento HTML.
Crear un formulario con los siguientes campos:
Nombre del producto
Cantidad
Precio unitario
Precio total
Dirección de envío
Información de contacto (nombre, correo electrónico, número de teléfono)
Agregar los siguientes campos relacionados al formulario:
Método de pago
Fecha de entrega
Comentarios
Utilizar las etiquetas HTML apropiados para cada campo.



### Solución

<!DOCTYPE html>

<body>
    <head>
    <form action="example.php">

         
            <h1>FORMULARIO DE NOMBRE</h1>

            <br>
            <br>
        
        <div>
            
        <label for="idnombreproducto"><strong>NOMBRE DEL PRODUCTO:</strong></label>
        <input type="text" name="nombreproducto" id="idnombreproducto" placeholder="nombre del producto">
    </div>
    <br>

    <div>
        <label for="idCantidad"><strong>CANTIDAD:</strong></label>
        <input type="number" name="cantidad" id="idCantidad" placeholder="cantidad">
    </div>
    <br>
    
    <div>
        <label for="idPrecio Unitario"><strong>PRECIO UNITARIO:</strong></label>
        <input type="number" name="Precio Unitario" id="idPrecio Unitario" placeholder="Precio Unitario">
    </div>   
    <br>
    
    <div>
        <label for="idPrecio Total"><strong>PRECIO TOTAL:</strong></label>
        <input type="number" name="Precio Total" id="idPrecio Total" placeholder="Precio Total">
    </div>   
    <br>
    
    <div>
        <label for="idDireccion del envio"><strong>DIRECCION DEL ENVIO:</strong></label>
        <input type="text" name="Direccion del envio" id="idDireccion del envio" placeholder="Direccion del envio">
    </div>   
    <br>
    <br>
    <br>
    <br>
 
        <h2>INFORMACIÓN DE CONTACTO</h2>

        <br>
        <br>

        <div>
            <label for="idnombredelcliente"><strong>NOMBRE DEL CLIENTE:</strong></label>
            <input type="text" name="nombreproducto" id="idnombredelcliente" placeholder="Nombre del cliente">
        </div>
        <br>

        <div>
            <label for="idNúmerodeCédula"><strong>NÚMERO DE CÉDULA:</strong></label>
            <input type="text" name="idNúmerodeCédula" id="idNúmerodeCédula" placeholder="Número de Cédula" autocomplete="off">
        </div>
        <br>

        <div>
        <label for="idcorreoelectronico"><strong>CORREO ELECTRONICO:</strong></label>
        <input type="email" name="correoelectronico" id="idcorreoelectronico" placeholder="Correo electrónico">
    </div>
    <br>

    <div>
        <label for="idNumero telefonico"><strong>NÚMERO TELEFONICO:</strong></label>
        <input type="tel" name="Numero telefonico" id="idNumero telefonico" placeholder="Numero telefonico">
    </div>   
    <br>

    <h2>MEDIOS DE PAGO</h2>

    <div>

    <select name="Tipodetarjeta" id="Tipo de tarjeta">
        <option value="VISA">VISA</option>
        <option value="MASTERCARD" selected>MASTERCARD</option>
        <option value="AMERICAN EXPRESS">AMERICAN EXPRESS</option>
        <option value="BANCOLOMBIA">BANCOLOMBIA</option>
    </select>

    </div>

    <br>
       
    <div>
    <label for="idfechayhora"><strong>FECHA Y HORA DE ENTREGA:</strong></label>
    <input type="datetime-local" name="fechayhora" id="idfechayhora">
    </div>   
    <br>
        
    <div>
    <textarea name="comentarios" id="comentarios" placeholder="Ingrese sus comentarios aquí" rows="10" cols="50"></textarea>
    </div>
        
        <input type="submit" value="Enviar">
    </div>   
    <br>

      </form>
    <br>

    </head>
    </body>
    </html>
       


