Diferencia entre CMD y ENTRYPOINT:

La instrucción ENTRYPOINT establece el ejecutable que utilizará el proceso del contenedor Docker, si no se utiliza en el Dockerfile entonces Docker utiliza el ENTRYPOINT por defecto q es "/bin/sh
 -c".

ENTRYPOINT ["/bin/echo"]


La instrucción CMD en cambio establece los parámetros a usar del ejecutable definido en ENTRYPOINT, estos parámetros pueden ejecutar ejecutables.

CMD ["Hello"]

En este caso le pasamos un argumento al ejecutable de ENTRYPOINT, si hacemos build del Dockerfile y run del contenedor sacará por consola el texto "Hello".