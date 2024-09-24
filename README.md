# Proyecto IoT para el Monitoreo de Cámaras Frigoríficas en Restaurantes

## Descripción General
Este proyecto tiene como objetivo desarrollar un sistema de monitoreo IoT para controlar la **temperatura** y **humedad** en la cámara frigorífica del restaurante **Le Boucher**, dedicado a conservar carne vacuna envasada al vacío. El sistema está basado en un microcontrolador **ESP32** que gestiona sensores de temperatura y humedad (**DHT22**) y varios actuadores, como un buzzer y LEDs, para alertar sobre condiciones anormales. Además, se integra con la plataforma en la nube **Azure IoT** para procesar y analizar los datos en tiempo real.

## Características Principales
- **Monitoreo Ambiental**: El sistema mide continuamente la temperatura y humedad dentro de la cámara frigorífica.
- **Alertas Automáticas**: Genera alertas visuales (LEDs) y sonoras (buzzer) cuando los parámetros están fuera de los rangos establecidos.
- **Conexión a la Nube**: Los datos se envían a **Azure IoT Hub** mediante el protocolo **MQTT** para su procesamiento y almacenamiento.
- **Procesamiento en Tiempo Real**: **Azure Stream Analytics** procesa los datos en tiempo real, detectando condiciones críticas.
- **Almacenamiento de Datos**: Se utiliza **Azure SQL Database** para almacenar los datos históricos de los sensores.
- **Visualización**: El sistema permite visualizar datos en **dashboards interactivos** mediante **Power BI**.
- **Seguridad**: **Azure Security Center** monitorea la seguridad de los dispositivos IoT y la comunicación con la nube, detectando vulnerabilidades y cifrando los datos.

## Arquitectura del Sistema
La arquitectura consta de los siguientes componentes clave:
1. **Microcontrolador**: **ESP32**, que gestiona los sensores y actuadores y envía los datos a la nube.
2. **Sensores**: **DHT22** para medir temperatura y humedad.
3. **Actuadores**: **Buzzer** para alertas sonoras y **LEDs** para indicaciones visuales.
4. **Protocolo de Comunicación**: **MQTT** para transmitir los datos desde el ESP32 hacia la nube.
5. **Plataforma en la Nube**:
   - **Azure IoT Hub**: Gestiona los dispositivos IoT y la transmisión de datos.
   - **Azure Stream Analytics**: Procesa los datos en tiempo real.
   - **Azure SQL Database**: Almacena los datos recolectados para su análisis posterior.
   - **Azure Functions**: Ejecuta acciones automáticas, como el envío de alertas.
   - **Power BI**: Permite la visualización de los datos recolectados.
   - **Azure Security Center**: Asegura la comunicación y protege los dispositivos IoT.

## Desarrollo del Hardware
El hardware fue simulado utilizando la plataforma **Wokwi**, donde el microcontrolador ESP32 fue programado en **C++** para gestionar los sensores y actuadores. El montaje físico será realizado posteriormente en la fase final del proyecto.

## Implementación de la Plataforma en la Nube
Los datos recolectados se envían a **Azure IoT Hub** utilizando **MQTT**, donde se gestionan los dispositivos y se procesan los datos en tiempo real con **Azure Stream Analytics**. Los datos históricos se almacenan en **Azure SQL Database** y se muestran en **Power BI** para permitir una visualización interactiva.

## Integración de IoT y Cloud Computing
El sistema combina IoT y Cloud Computing para ofrecer una solución integral, procesando y analizando datos en tiempo real. Se han creado **dashboards** que permiten al personal del restaurante supervisar las condiciones de la cámara frigorífica de manera remota, y las alertas automáticas se activan cuando se detectan problemas.
Además, se ha implementado un sistema de **seguridad** robusto mediante **Azure Security Center**, que protege la infraestructura y asegura las comunicaciones.

## Estado Actual del Proyecto
El proyecto se encuentra en la fase final de desarrollo, con el hardware y la plataforma en la nube casi completamente integrados. El sistema ha sido probado en simulaciones, y las siguientes fases incluyen la implementación física y la configuración de las últimas medidas de seguridad.

## Próximos Pasos
- Finalizar la configuración de la infraestructura en la nube.
- Implementar pruebas finales del sistema en hardware real.
- Desplegar el sistema en la cámara frigorífica del restaurante **Le Boucher**.
- Capacitar al personal del restaurante para el uso del sistema.

## Conclusión
Este proyecto de monitoreo IoT proporciona una solución integral para la gestión de cámaras frigoríficas en restaurantes. Integra tecnología IoT con procesamiento en la nube y medidas de seguridad, optimizando el control de la calidad del producto y la eficiencia operativa.

## Contacto
Para más información o consultas:
- **Cristian Ghisiglieri** - [cristian.g2011@gmail.com](mailto:cristian.g2011@gmail.com)
- **Germán Liendo** - [g3rm6n@gmail.com](mailto:g3rm6n@gmail.com)
- **Naylui Osuna** - [nayluiosuna@gmail.com](mailto:nayluiosuna@gmail.com)
- **Romina Peña** - [rominabpena@gmail.com](mailto:rominabpena@gmail.com)
