# Practica-Refactorizacion
1. Renombrado de variables y método
Elemento
original
Nuevo nombre
p procesarFactura
l precios
t total
n nombreCliente
imp Impuesto
Procedimiento:
1. Seleccionar el identificador
2. Pulsar Alt + Shift + R
3. Escribir el nuevo nombre
4. Confirmar con Enter
2. Extracción de método: cálculo de suma (Extract
Method)
Se ha extraído el bucle for a un método independiente llamado calcularSumaBase.
Procedimiento:
1. Seleccionar el bloque for
2. Pulsar Alt + Shift + M
3. Introducir el nombre del método
4. Ajustar el tipo de retorno a double
3. Extracción de método: lógica de negocio
Se ha extraído la lógica de descuentos e impuestos a un método llamado
aplicarDescuentoOImpuesto.
Procedimiento:
1. Seleccionar el bloque if-else
2. Pulsar Alt + Shift + M
3. Nombrar el método
4. Añadir parámetros necesarios (total, impuesto, esVip)
5. Ajustar retorno
4. Eliminación de código duplicado
Se ha detectado código duplicado en las instrucciones System.out.println.
Se ha creado el método imprimirResultado.
Procedimiento:
1. Seleccionar únicamente las líneas System.out.println
2. Pulsar Alt + Shift + M
3. Nombrar el método
4. Añadir parámetros (nombreCliente, total)
5. Eliminación de números mágicos
El valor 0.10 se ha sustituido por una constante:
Procedimiento:
1. Seleccionar 0.10
2. Ir a Refactor → Extract Constant
3. Nombrar la constante
4. Definirla como private static final
