<img align="right" width="45%" alt="Logo ORT" src="https://bg-so-1.zippyimage.com/2023/10/24/cfcf73422f9564677706d65737c0e189.png" />

# Proyecto Integrador
## Analista en Tecnologías de la Información
#### Septiembre 2023 - Abril 2024

<br/>
<br/>
<br/>

# Ampliación de sistema piloto de permisos de construcción digitales para la Intendencia de Montevideo.
### Autores: Nicolás Fernández - Sebastián Paulos
### `Calificación: 90/100`

<img align="right" width="70%" alt="Entrega Final" src="https://github.com/pi-ati-ort/.github/assets/82982815/cbd26f2a-9f81-4789-80b6-4267d8222683" />

## Contenido

1. [Abstract](#abstract)
2. [Necesidades y Objetivos](#necesidades-y-objetivos)
3. [Solución Propuesta](#solución-propuesta)
4. [Requerimientos](#requerimientos)
5. [Cronograma](#cronograma)
6. [Demo](#demo)
7. [Subsistemas](#subsistemas)
8. [Casos de Uso](#casos-de-uso)
9. [Instalación](#instalación)
10. [Documento](#documento)

<br/>
<br/>
<hr/>

## Abstract

El proyecto final de carrera se enfoca en la expansión de un proyecto existente, el cual tiene como objetivo principal la implementación de un sistema de gestión de permisos de construcción digitales en la Intendencia de Montevideo (IdeM). Este proyecto busca abordar una serie de desafíos en la gestión de permisos de construcción, relativos a los procesos de solicitud, evaluación y aprobación de estos. 


Para abordar estos desafíos, se ha desarrollado un piloto que permite la recepción de archivos IFC (Industry Foundation Class), un estándar de exportación de modelos digitales BIM (Building Information Modeling), lo que permite verificar si los modelos cumplen con la normativa vigente a través de algoritmos y cálculos geométricos. El piloto actualmente cubre una parte del Digesto Departamental. 


El alcance del proyecto incluye la creación de un sistema conservando los lenguajes utilizados en el piloto, compuesto por diversos subsistemas, como un servidor BIM para el almacenamiento de modelos IFC y un subsistema Frontend que permite la visualización e interacción con modelos 3D. La inclusión de un Motor DMN (Decision Model and Notation) para abordar requerimientos normativos como reglas de negocio. También implica el establecimiento de una nueva base de datos para almacenar información procesada, y un subsistema Backend para gestionar la comunicación interna y externa de los nuevos módulos del sistema.


En resumen, el proyecto tiene como objetivo aportar valor incorporando nuevas funcionalidades, destacando el Servidor BIM, mejorando la eficiencia y la calidad en la gestión de permisos de construcción en la IdeM a través de la digitalización y la modernización de procesos, lo que contribuirá a una administración más eficiente y transparente en este ámbito. Además, reconoce el potencial de futuras expansiones y mejoras a medida que se implementa la solución final definitiva.

<br/>
<hr/>

## Necesidades y Objetivos

### Necesidades


- Implementar un servidor BIM para cargar y procesar los archivos IFC.
- Incorporar una nueva interfaz de usuario con dos roles con distintas funcionalidades, el de Arquitecto y el de Administrador.
- Incorporar una interfaz gráfica que permita visualizar modelos 3D para su análisis.
- Incorporar conceptos normativos mediante algoritmos de modelado y cálculo, bajo el estándar DMN.
- Implementar una arquitectura del sistema que permita dar soporte y conexión a todas las necesidades descritas anteriormente. 


### Objetivos

- Desarrollar un sistema de gestión de permisos de construcción que automatice procesos, reduzca errores y ambigüedades en la normativa vigente.
- Garantizar la aplicación precisa y coherente de las regulaciones municipales de construcción incorporadas al sistema, mediante la implementación efectiva de la tecnología.
- Agilizar una parte del proceso de solicitud y aprobación de permisos, la revisión técnica de planos de arquitectura, reduciendo drásticamente los tiempos de respuesta a los profesionales actuantes.
- Aprender y dominar nuevas tecnologías requeridas para el éxito del proyecto, lo que permitirá un crecimiento profesional significativo.
- Contribuir al cambio tecnológico en el sector AEC (Architecture Engineering and Construction) al facilitar una herramienta que posiciona y beneficia el uso de BIM en el sector, desde un ente público.

<br/>
<hr/>

## Solución Propuesta

### Diagrama de Domino

<img width="50%" align="left" alt="Diagrama de Dominio" src="https://github.com/pi-ati-ort/.github/assets/82982815/bf22f381-be54-4744-9d06-e0203fc00925">

El diagrama de dominio presentado describe las entidades y relaciones involucradas en la gestión de este proyecto.

 **Usuario**<br/>
Representa al usuario de rol Arquitecto o Administrador que utiliza el sistema BIM. El usuario tiene un identificador único (id), un nombre, un nombre de usuario y una contraseña, y un rol, entre otras cosas.

 **Proyecto**<br/>
 Es un conjunto de datos y recursos sobre la construcción. El proyecto tiene un nombre, una descripción, un esquema, una dirección, un padrón, un identificador BIM y un identificador único universal (uuid), entre otras cosas.

 **Modelo**<br/>
 Es una representación digital de la construccion de un edificio.

<br/>
<br/>
<br/>
<br/>

### Diagrama de Diseño

<img width="100%" alt="Diagrama de Diseño" src="https://github.com/pi-ati-ort/.github/assets/82982815/08b423ea-f8ee-486e-8470-f4b8c1594445">

<br/>
<br/>
<hr/>

## Requerimientos

**Sistema de acceso** <br/>
Un sistema que permita el acceso a múltiples usuarios, que permita acceder a distintas funcionalidades de acuerdo con su rol. Se plantea dentro del alcance de este trabajo dos roles: Arquitecto y Administrador.


**Carga de archivos IFC a través de BIM** <br/>
Establecer un sistema, a través de un servidor BIM, que permita la carga de archivos en el estándar IFC, mediante una estructura de Proyectos y Modelos.

**Incorporación de normativas en estándar DMN** <br/>
Implementar un sistema que permita la validación de normativas a través del estándar DMN. Se incorporarán requerimientos normativos para ser analizados y verificados en los modelos.

**Análisis y verificación normativa de modelos IFC** <br/>
Permitir el análisis normativo del modelo IFC para corroborar que la edificación involucrada en el permiso de construcción cumple la normativa especificada.

**Visualización 3D del modelo IFC** <br/>
Se incorporará un sistema que permitirá visualizar e interactuar con diseños en 3D, mejorando la transparencia y la comunicación efectiva entre los profesionales solicitantes y los funcionarios, lo que mejorará la comprensión, la eficiencia y la precisión en el proceso de aprobación de permisos de construcción.

<br/>
<hr/>

## Cronograma

Para la planificación se utilizo GitHub Projects. Se puede consultar el cronograma con todas las tareas del proyecto [acá](https://github.com/orgs/pi-ati-ort/projects/4).

<hr/>

## Demo

https://github.com/pi-ati-ort/.github/assets/82982815/cfcd348a-8cdb-46f5-b0d0-1884d6ce7c1c

<br/>
<hr/>

## Subsistemas

**Backend** [https://pi-ati-back-backend.azuremicroservices.io/swagger-ui/index.html](https://pi-ati-back-backend.azuremicroservices.io/swagger-ui/index.html)

**Frontend** [https://pi-ati-ort-front.vercel.app/](https://pi-ati-ort-front.vercel.app/)

**BIM Server** [http://18.215.219.56:8082/](http://18.215.219.56:8082/)

**DB** [postgresql://pidb.c5i2i6o6q7jl.us-east-1.rds.amazonaws.com:5432](postgresql://pidb.c5i2i6o6q7jl.us-east-1.rds.amazonaws.com:5432)

**DMN Server** [https://jbpm-dmn.eastus2.azurecontainer.io/business-central/kie-wb.jsp](https://jbpm-dmn.eastus2.azurecontainer.io/business-central/kie-wb.jsp)
<br/>
*En local en localhost:8080/busin...*

<hr/>

## Casos de Uso

### Sistema de Acceso

https://github.com/pi-ati-ort/.github/assets/82982815/16ff11a3-e65f-434e-988c-d93787595d22

### Rol Arquitecto

https://github.com/pi-ati-ort/.github/assets/82982815/c2376d21-2608-486a-9924-2f8bd2836716

### Rol Administrador

https://github.com/pi-ati-ort/.github/assets/82982815/708abc53-f619-4b8c-814e-09a010cf6460

<br/>
<hr/>

## Instalación

Aquí se explicará como ejecutar los subsistemas localmente para probar correctamente todas las funcionalidades de la aplicación. 

*En proceso...*

<br/>
<hr/>

## Documento

Puedes consultar el documento final entregado [acá](https://nicolasfuy.s3.amazonaws.com/documentos/TESIS-ATI.pdf).
<br/>
