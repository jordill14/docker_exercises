Hago el build en la carpteta que tengo el Dockerfile, arrancamos un contenedor y vamos mirando el estado del contenedor:

![alt text](https://github.com/jordill14/docker_exercises/blob/main/hw-04/images/healthy.PNG)


Parámetros de HEALTHCHECK:

Prueba cada 45s: --interval=45s 

Se espera que responda en 5s sino falla: --timeout=5s 

Ajustar el tiempo para la primera prueba: --start-period=15s 

Número de reintentos: --retries=2
