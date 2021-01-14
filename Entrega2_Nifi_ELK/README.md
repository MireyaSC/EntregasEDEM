# ENTREGA EJERCICIO 2: Nifi + ELK

Usando nifi+ELK debéis presentar una solución que muestre sobre un mapa la disposición de delitos presentes en esta api: 
https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9

## Entregables:
•	Enlace a código Github
•	Captura de pantalla de vuestra interfaz Kibana

## Opcional:
•	Existen otras fuentes de datos que proporcionan también llamadas al 311 de otras zonas, opcionalmente podéis concatenar más datasets y pintarlos de manera conjunta.
https://catalog.data.gov/dataset/311-data-in-development

# PASOS SEGUIDOS PARA LA REALIZACIÓN DEL EJERCIO

## Primero: Generar un fichero docker-compose.yml con Nifi, Elasticsearch y Kibana:

https://github.com/MireyaSC/EntregasEDEM/blob/main/Entrega2_Nifi_ELK/Code/docker-compose.yml

## Segundo: hacemos un flujo en Nifi configurando los procesadores así:

    ### Elegimos un procesador del tipo InvokeHTTP para poder ingestar datos con el API: 

