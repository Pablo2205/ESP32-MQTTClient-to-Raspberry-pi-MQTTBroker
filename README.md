# ESP32 MQTT Client publisher Raspberry pi MQTT Broker 

Este proyecto muestra cómo utilizar el protocolo de comunicación MQTT con ESP32 para publicar mensajes y suscribirse a temas. Como ejemplo, publicamos los valores del sensor BME280 en el tablero de Node-RED y controlamos una salida ESP32. Programamos el ESP32 con Arduino IDE.

<img width="828" height="466" alt="image" src="https://github.com/user-attachments/assets/0e3e5b25-0199-41ee-adc1-50fcc0f2091c" />


En este ejemplo, hay una aplicación Node-RED que controla las salidas de ESP32 y recibe valores de sensores de ESP32 a través del protocolo de comunicación MQTT. La aplicación Node-RED se ejecuta en una Raspberry Pi.

Usamos el broker Mosquitto instalado en la misma Raspberry Pi. El corredor es responsable de recibir todos los mensajes, filtrarlos, decidir quién está interesado en ellos y publicarlos para todos los clientes suscritos.

La siguiente imagen muestra una descripción general de lo que haremos en este tutorial.

<img width="800" height="425" alt="image" src="https://github.com/user-attachments/assets/50a26538-5e33-4571-a235-9e59e670cf17" />

ESP32 MQTT: publicar y suscribirse con Arduino IDE
La aplicación Node-RED publica noticias (“En» o «fuera de«) en tema esp32/problema. El ESP32 está suscrito a este tema. Entonces recibe el mensaje con “on” o “off” para encender o apagar el LED.
El ESP32 da la temperatura en el esp32/temperatura El tema y la humedad en el esp32/humedad Tema. La aplicación Node-RED está suscrita a estos temas. Esto le proporciona valores de temperatura y humedad que se pueden representar, por ejemplo, en un diagrama o en una pantalla.
Nota: También hay un tutorial similar sobre el uso de ESP8266 y Node-RED con MQTT.

requisitos
Deberías estar familiarizado con Raspberry Pi; lee Introducción a Raspberry Pi.
Debe tener el sistema operativo Raspbian instalado en su Raspberry Pi; lea «Instalar, activar y conectar Raspbian Lite usando SSH».
Debe tener Node-RED instalado en su Pi y Node-RED Dashboard.
Aprenda qué es MQTT y cómo funciona.
Si te gusta la domótica y quieres aprender más sobre Node-RED, Raspberry Pi, ESP8266 y Arduino, te recomendamos nuestro curso: Crear un sistema domótico con Node-RED, ESP8266 y Arduino. También tenemos un curso específico para ESP32: Regístrate en el curso Aprende ESP32 con Arduino IDE.

Piezas requeridas
Estas son las piezas necesarias para construir el circuito (haga clic en los enlaces a continuación para encontrar el mejor precio en Asesor de creadores):

ESP32 MQTT: publicar y suscribirse con Arduino IDE
Raspberry Pi
Placa ESP32 DOIT DEVKIT V1
Módulo de sensores BME280
1 LED de 5 mm
1x resistencia de 220 ohmios
tablero de circuitos
Cables de puente

<img width="750" height="460" alt="image" src="https://github.com/user-attachments/assets/f349c0fe-453f-4ce6-bd83-9f8e4bd60609" />
