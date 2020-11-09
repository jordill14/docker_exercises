Diferencia entre COPY y ADD:

COPY:

La instrucción COPY solo se encarga de copiar un archivo de nuestro equipo local y añadirlo a la imagen Docker en la que estamos trabajando.

COPY fuente destino

ADD:

En cambio la instrucción ADD a parte de copiar un archivo local, también te permite la extracción de archivos “.tar” en local e indicar contenidos vía URL.

En definitiva, la instrucción ADD hace lo mismo que la instrucción COPY pero añade dos funcionalidades que el COPY no tiene.

ADD http://example.com/directorio /usr/local/remote/

ADD recursos/jdk-7u79-linux-x64.tar.gz /usr/local/tar/