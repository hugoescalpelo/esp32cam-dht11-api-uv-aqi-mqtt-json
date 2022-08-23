# esp32cam-dht11-g7
Este repositorio contiene los archivos para el ejercicio en clase que envía la información del DHT11 por MQTT a NodeRed

Este ejercicio consiste en realizar una estación de clima que realice lo siguiente:
- Obtener información de temperatura y humedad relativa del sensor Dhttps://docs.google.com/spreadsheets/d/1s_RaDnrUEG3wdS_fm7fdf1gNFYoXVmumj7km8WwM8m0/edit?usp=sharingHT11 con el micro controlador ESP32CAM
- Enviar los valores del sensor por MQTT de forma local en JSON, con el objetivo de enviar varias variables en el mismo mensaje
- Generar un Flow que obtenga por MQTT los valores enviados por el sensor y realice una gráfica del historico y muestre indicadores de valores instantaneos
- Generar un flow, basado en el [flow 5](https://github.com/hugoescalpelo/flow5-openweather-g7), el cual realice lo siguiente
    - Obtener valor de temperatura, humedad relativa, Calidad del Aire, Indice Ultra Violeta por API de openweathermap.org
    - Graficar valores instantaneos e historicos del la ubicación actual en un dashboard
    - Suscribirse a un Broker MQTT público para poder obtener la información de datos climáticos de todos los alumnos del grupo 7
    - Reportar por MQTT los datos obtenidos por API para que puedan ser visualizados por el resto de los alumnos


## Modificaciones a realizar

- Modificar Coordenadas geograficas para obtener los datos climaticos por API
- Modificar la API Key para poder obtener información de openweathermap.org
- Temas MQTT locales y publicos donde se reportan los datos obtenidos por API y por sensores

# Vista previa del resultado

![Vista previa](https://github.com/hugoescalpelo/esp32cam-dht11-g7/blob/main/Dashboard%20estacion%20climatica%20API%20y%20Sensores.png?raw=true)