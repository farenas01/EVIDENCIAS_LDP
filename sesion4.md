<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


Actividad: Crear una tabla HTML con información sobre productos.
Escribir una tabla HTML con 10 filas que muestre información sobre productos reales. La tabla debe tener las siguientes columnas:

Código
Nombre
Descripción
Precio
Stock
Fecha de creación
Además, combinar celdas en la tabla con los atributos rowspan y colspan, como se muestra en la siguiente imagen.

### Solución

    <table border="5" cellpadding="3" cellspacing="10">
    <thead>
    <tr>
      <th>Código</th>
      <th>Nombre</th>
      <th colspan="2">Descripción</th>
      <th>Precio</th>
      <th>Stock</th>
      <th>Fecha de creación</th>
      <th>Lugar de creación</th>
      <th>Ubicación</th>
      <th>Estado</th>
      <th>Garantía</th>

    </tr>

    </thead>
    <tbody>
    <tr>
      <td rowspan="2">23456</td>
      <td rowspan="2">COMPUTADOR PORTATIL.</td>
      <td colspan="2">Computador portatil core i6 de 10g, con 8 gigas de memoria ram.<br>Marca ASUS</td>
      <td>$2.500.000<br><strong>PESOS</strong></td>
      <td>1742<br><strong>UNIDADES</strong></td>
      <td>15/12/23</td>
      <td>MEDELLIN,<br>COLOMBIA</td>
      <td>BODEGA.<br>78</td>
      <td>NUEVO.</td>
      <td>2 AÑOS A NIVEL MUNDIAL.<br><strong>NO APLICA PARA MAL USO...</strong></td>


    </thead>
  <tbody>
    <tr>
      <td rowspan="2">21234</td>
      <td rowspan="2">TELEVISOR SMART TV.</td>
      <td colspan="2">Tv Smart tv de 70 pulgadas marca Samsung.<br>Control inteligente por mando de voz</td>
      <td rowspan="2">$3.800.000<br><strong>PESOS</strong></td>
      <td rowspan="2">512<br><strong>UNIDADES</strong></td>
      <td rowspan="2">11/06/23</td>
      <td rowspan="2">MEDELLIN,<br>COLOMBIA</td>
      <td rowspan="2">BODEGA.<br>32</td>
      <td rowspan="2">DE EXHICICIÓN.</td>
      <td rowspan="2">1 AÑO Y MEDIO</td>

    </tr>

    <tr>
      <td colspan="2">Puedes comprar adicionalmente un teatro en casa complementario.</td>
    </tr>

    </thead>
  <tbody>
    <tr>
      <td rowspan="2">42134</td>
      <td rowspan="2">MINICOMPONENTE.</td>
      <td colspan="2">Dispositivo auditivo marca LG color negro, de 1200 watts de sonido.<br>Reconocimiento de voz.</td>
      <td>$1.300.000<br><strong>PESOS</strong></td>
      <td>7654<br><strong>UNIDADES</strong></td>
      <td>25/08/23</td>
      <td>MEDELLIN,<br>COLOMBIA</td>
      <td>BODEGA.<br>21</td>
      <td>NUEVO</td>
      <td>1 AÑO.<br>ADICIONAL PUEDES COMPRAR UN SEGURO CONTRA ROBO.</td>

    </tr>

    </thead>
  <tbody>
    <tr>
      <td rowspan="2">98001</td>
      <td rowspan="2">ESTUFA HACEB.</td>
      <td colspan="2">Estufa electrica marca haceb, para uso con implementos de cocina especiales.</td>
      <td rowspan="2">$1.800.000<br><strong>PESOS</strong></td>
      <td rowspan="2">1742<br><strong>UNIDADES</strong></td>
      <td rowspan="2">15/12/23</td>
      <td rowspan="2">MEDELLIN,<br>COLOMBIA</td>
      <td rowspan="2">BODEGA.<br>19</td>
      <td rowspan="2">NUEVA<br><strong>IMPORTADA</strong></td>
      <td rowspan="2">2 AÑOS</td>

    </tr>

    <tr>
      <td colspan="2">Por la compra de la estufa te obsequiamos un juego de ollas.</td>
    </tr>

  </tbody>
    
</thead>
  <tbody>
    <tr>
      <td rowspan="2">42324</td>
      <td rowspan="2">HORNO MICROONDAS.</td>
      <td colspan="2">Horno microondas marca haceb de 1200 watts de energia.<br>Lector de huella.</td>
      <td>$1.100.000<br><strong>PESOS</strong></td>
      <td>656<br><strong>UNIDADES</strong></td>
      <td>25/12/23</td>
      <td>MEDELLIN,<br>COLOMBIA</td>
      <td>BODEGA.<br>01</td>
      <td>NUEVO</td>
      <td>1 AÑO Y MEDIO.</td>

    </tr>

    </thead>
  <tbody>
    <tr>
      <td rowspan="2">14321</td>
      <td rowspan="2">CELULAR HUAWEI P 40</td>
      <td colspan="2">Dispositivo movil marca huawei de 16 gigas de RAM</td>
      <td rowspan="2">$3.800.000<br><strong>PESOS</strong></td>
      <td rowspan="2">1200<br><strong>UNIDADES</strong></td>
      <td rowspan="2">01/09/23</td>
      <td rowspan="2">MEDELLIN,<br>COLOMBIA</td>
      <td rowspan="2">BODEGA.<br>19</td>
      <td rowspan="2">NUEVO<br><strong>IMPORTADA</strong></td>
      <td rowspan="2">2 AÑOS</td>

    </tr>

    <tr>
      <td colspan="2">Disponible en colores gris, negro y dorado.</td>
    </tr>

  </tbody>
</table>





