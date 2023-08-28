#

## Implemetación whatsapp web servidor Kamatera

Pasos para ejecutarlo en el ambiente:

1. Pasar el archivo comprimido **Fuentes.zip** a la carpeta `/opt`
2. Descomprimir el archivo **Fuentes.zip** en la misma carpeta `/opt`
3. Para evitar error de escritura utilizar el seguiente comando ->
   `chmod 777 -R /opt/Fuentes`
4. Ejecutar el comando -> `docker-compose build`
5. Ejecutar el comando `docker-compose up` y Esperar que termine de instalar y levantar los 3 servicios definidos en el archivo **docker-compose.yml**
6. Una vez los servicios se estén ejecutando,abrir una segunda terminal e ingresar al contenedor de node con el siguiente comando -> `docker exec -it fuentes_node_1 sh`
7. Instalar las dependencias del proyecto nodejs con el comando -> `npm i`
8. Ejecutar la app de whatsapp con el comando ->` node index.js`
9. Despues de un momento aparece en la consola el qr cada cierto tiempo.
