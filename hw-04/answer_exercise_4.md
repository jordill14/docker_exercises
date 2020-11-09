Hago el build en la carpteta que tengo el Dockerfile con las instrucciones y arrancamos un contenedor:

![alt text](https://github.com/jordill14/docker_exercises/blob/main/hw-04/images/Dockerfile_healthcheck.PNG)

Fallan dos pruebas consecutivas con el parámetro a 15s y aparece como estado: "unhealthy"

![alt text](https://github.com/jordill14/docker_exercises/blob/main/hw-04/images/health.PNG)

Parámetros de HEALTHCHECK:

Prueba cada 45s: --interval=45s 

Se espera que responda en 5s sino falla: --timeout=5s 

Ajustar el tiempo para la primera prueba: --start-period=15s 

Número de reintentos: --retries=2
