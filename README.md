# TPO1
**Proyecto en Unity - Caza de Ingredientes para la Cafetería**

## 1. Idea
La idea que planteo para este trabajo es armar una app con para una cafetería. En esta experiencia en la que se utilizará realidad aumentada, los usuarios podrán interactuar con el entorno buscando y recogiendo un café virtual. Por medio de la cámara de su celular, los clientes deberán encontrar y capturar el objeto escondido en el local (cuando toque en su pantalla el objeto, desaparecerá dando a entender que lo cazó).

## 2. Relevamiento de requerimientos
**Objetivos del Proyecto**
Permitir que los usuarios recojan un café oculto en algún lugar en específico.

**Elementos Principales**
Entorno 3D e Interfaz
Modelos 3D de Cafés: Se utilizarán modelos simples descargados desde Unity Asset Store o Sketchfab.
Cámara de AR: La cámara del celular permitirá buscar el café en el entorno a través de realidad aumentada.

**Funcionalidad Principal**
Caza de Cafés: El café aparecerá en distintos puntos del local, simulando estar escondido. El usuario podrá capturarlo acercándose y haciendo clic sobre el objeto.

**Resumen de Características Técnicas**
Plataforma: Unity con integración de realidad aumentada.
Assets: Modelos 3D simples descargados desde Unity Asset Store o Sketchfab.
Interacción: Captura de objetos 3D mediante clic sobre los objetos visibles en la cámara.

## 3. Problemas en Unity
En el desarrollo del proyecto, tuve varias dificultades que afectaron la implementación. A continuación, detallo los problemas principales que encontré y los pasos que realicé para intentar resolverlos.

**Integración de la Cámara
Al iniciar el proyecto, uno de los mayores desafíos fue integrar la cámara para visualizar el objeto en realidad aumentada (en este caso, una taza de café). En un primer momento, logré que la cámara funcionara en el celular, pero no mostraba el objeto deseado. 

**Uso de Vuforia
Para mejorar la funcionalidad y lograr que el objeto (la taza de café) apareciera en la escena, decidí utilizar Vuforia, un software que permite crear aplicaciones de realidad aumentada en Unity. Para configurarlo, realicé los siguientes pasos:
-Instalación y configuración de Vuforia en Unity: Seguí el proceso según la página ofical de Vuforia.
-Creación de la License Key y Database: Generé una License Key en la página de Vuforia y configuré una base de datos con la imagen de referencia que permitiría a la cámara detectar el objeto. Esta imagen de referencia debía activar la visualización de la taza de café en la pantalla cuando se enfocara.

**Problemas de Compilación y Ejecución
A pesar de configurar Vuforia, surgieron otros problemas:
-Logré que el celular abriera la aplicación de Unity pero al probarla, no mostraba la cámara, por ende tampoco se veía el objeto.
