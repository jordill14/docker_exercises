Diferencia entre CMD y ENV:

La instrucción ENV establece unas variables de entorno persistentes dentro de nuestro contenedor, estás serán visibles para las siguientes instrucciones.

ENV <key> <value>

La instrucción CMD no solo puede establecer unas variables por defecto sino que puede ejecutar ejecutables, las variables o ejecutables que se pasan por medio de esta instrucción se ejecutan una vez que el contenedor se ha inicializado.

CMD [“ejecutable”, “parametro1”, “parametro2”, …]