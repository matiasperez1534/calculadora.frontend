Creamos el archivo funciones.js para luego enlazarlo con un script en el html index.html dentro del body.

agregamos el framework Bootstrap por medio de cdn , ademas del css por medio de link.

añadimos un header con el titulo del proyecto  .
creamos un div para centrar el container, luego dejaremos en un main otro container.

seguimos con otros 2 div para la fila "row" y "col" , ademas le agregamos un "input" para visualizar los valores que estaremos ingresando con un identificador "id".

crearemos otros 4 div que contendran nuestros primeros 4 botones, entonces añadimos fila y columnas a la cual las identificaremos como "b1" "b2" "b3" y "bplus". centramos el texto en nuestro main y en cada boton le agregamos en class p-4 (padding) para distribuir visualmente mejor el boton y modificamos la clase del boton bplus a primary para diferenciar visualmente su función especial.
replicamos lo mismo para las 3 otras filas y columnas modificamos los id ("b4", "b5","b6", "bminus","b7", "b8","b9", "bmultiply" ,"bclean", "b0","bequal", "bdiv").

en el archivo funciones.js 

originamos en primera instancia la variable botonesNum para identificar los botones que tienen numero. hacemos que busque en el documento con getElementsByClassname ("btn btn-dark).

concebiremos la variable botonesAccion y hacemos que busque en el documento con getElementsByClassname ("btn btn-secondary).

*definiremos la variable botonesOperacion y hacemos que busque en el documento con getElementsByClassname ("btn btn-primary)

Seguimos para que este boton de operacion ejecute una accion con el evento onclick , para ello declaramos la variable limpiar y hacemos que busque en el documento con getElementsById ("bclean") luego seguimos con la variable agregandole el evento (addEventListener('click', clean) con lo que al hacer click llamara a la funcion clean, la cual generaremos a continuación :

definimos la variable tresultado y hacemos que busque en el documento con getElementsById ("resultado") con lo que accedera al input , seguimos con la variable añadiendole un value vacio (''). 

repetimos el proceso para el igual cambiando los identificadores asociados y agregando la funcion javascript eval para el tresultado.value.



estableceremos las condiciones de los botones numericos

empezaremos con el  bucle 'for' en el modificamos el array por nuestra variable botonesNum y definimos nuestra variable de control (index o i) que parta en 0 y va subiendo de 1 en 1 ('i++), en la constante modificar también por botonesNum, le añadimos el evento click y hacemos que llame a una función anonima que contiene a la funcion putNumber definiendole que es un elemento inerte de texto


*/ 
     funcion anonima es una funcion desechable que solo se llama una vez y nos sirve para que el navegador ejecute la función al realizar tal acción.


Generamos la funcion putNumber le damos valor a esta funcion,hacemos que concatene el tresutaldo.value += valor

repetimos el proceso para la condicion de operacion.