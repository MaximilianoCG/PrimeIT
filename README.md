MANUAL DE USUARIO Y DOCUMENTACIÓN DEL SISTEMA
PRIME IT

Elaborado por:
PRIME IT COMPANY
Carrera:
 Ingeniería en Sistemas de Computación Administrativa
Institución:
 TecMilenio
Materia:
Taller de productividad basada en herramientas tecnológicas

Versión del documento:
 1.0
Fecha de elaboración:
 05/05/2025

Tabla de Contenidos
Resumen Ejecutivo
 1.1 Descripción del sistema
 1.2 Problema identificado
 1.3 Solución propuesta
 1.4 Arquitectura del sistema
Requerimientos
 2.1 Servidor de aplicación
 2.2 Servidor web
 2.3 Base de datos
 2.4 Paquetes y dependencias adicionales
 2.5 Versiones de software (Java, frameworks, etc.)
Instalación
 3.1 Instalación del ambiente de desarrollo
 3.2 Ejecución de pruebas manuales
 3.3 Despliegue en ambiente local
 3.4 Despliegue en la nube (ej. Heroku)
Configuración
 4.1 Configuración del sistema
 4.2 Configuración de dependencias
Uso del Sistema
 5.1 Manual de usuario final
 5.2 Manual de administrador
Contribución
 6.1 Propósito
 6.2 Política de acceso al codigo
 6.3 Sugerencias
 6.4 Proceso de revisión y merge
Roadmap
 7.1 Estado actual del proyecto
 7.2 Solicitudes futuras
 7.3 Mantenimiento del sistema

Resumen ejecutivo

---Descripción del sistema---
La aplicación móvil de gestión de inventario es un sistema diseñado para apoyar las operaciones diarias de los empleados mediante una plataforma ágil, accesible y centralizada. Su propósito principal es permitir el registro, consulta y actualización de los productos en inventario en tiempo real, desde cualquier dispositivo móvil autorizado.
El sistema ofrece funcionalidades para capturar nuevos artículos, visualizar existencias disponibles, modificar cantidades, registrar entradas y salidas, así como mantener información actualizada sobre cada producto.
---Problema identificado---
RodaClean es una PYME con alto potencial de crecimiento; sin embargo, actualmente enfrenta importantes limitaciones debido a que sus procesos operativos se realizan de manera manual. La ausencia de sistemas digitales para la gestión de información provoca ineficiencias, mayor probabilidad de errores y dificultades en la organización interna.
Además, la empresa no cuenta con presencia digital, ya que carece de página web y redes sociales, lo que restringe significativamente su visibilidad en el mercado
---Solucion propuesta---

Se propone el desarrollo e implementación de un sistema digital de gestión de inventarios que permita registrar, controlar y dar seguimiento en tiempo real a las entradas y salidas de productos. Este sistema centralizará la información, facilitando el registro de movimientos, la consulta de existencias actuales y la actualización automática de cantidades disponibles. 

---Arquitectura del sistema---

La arquitectura del sistema se basa en una solución moderna tipo cliente–servidor, utilizando Android Studio para el desarrollo de la aplicación móvil y Firebase como plataforma backend en la nube. 

Capa de presentación (Frontend – Aplicación móvil):
Desarrollada en Android Studio, es la interfaz que utilizan los empleados. 
Capa de servicios (Backend – Firebase):
Firebase funciona como el backend del sistema dando a base de datos en tiempo real y autenticación.
Capa de datos:
Gestionada directamente por Firebase, donde se almacena toda la información relevante como productos, cantidades, movimientos (entradas/salidas) y usuarios. 

Requerimientos
–Servidor de aplicación–

El sistema utiliza Firebase como plataforma principal de servicios backend en la nube, encargándose de la autenticación de usuarios, sincronización de información y gestión de datos en tiempo real.

La aplicación móvil cliente fue desarrollada en Android Studio y se comunica directamente con los servicios proporcionados por Firebase mediante conexión segura a internet.

–Servidor web–

Actualmente, el sistema no requiere un servidor web tradicional dedicado, ya que la infraestructura en la nube de Firebase administra automáticamente los servicios necesarios para la comunicación entre la aplicación y la base de datos.

—Base de datos–

La solución utiliza Firebase Realtime Database como sistema de almacenamiento principal.

La base de datos permite:
Almacenar información de productos e inventario
Registrar entradas y salidas de productos
Gestionar usuario y roles
Mantener sincronización de información en tiempo real
Toda la información se encuentra centralizada y protegida mediante los mecanismos de seguridad proporcionados por Firebase.

–Paquetes adicionales–

Para el correcto funcionamiento del sistema, se utilizan distintas librerías y dependencias integradas durante el desarrollo de la aplicación móvil. Entre los principales se incluyen:
Firebase Authentication
Firebase Realtime Database
Firebase SDK para Android
Estas dependencias permiten implementar funcionalidades relacionadas con autenticación, almacenamiento de datos, interfaz gráfica y sincronización de información.

–Versiones de software–

Las principales tecnologías y versiones utilizadas durante el desarrollo del sistema son las siguientes:

Componente:
Android Studio
Java
Android SDK
Firebase SDK
Gradle
Material design

Version:
Panda 4
JDK 17
API 34
última versión estable
8.x
Última versión estable

Las versiones podrán actualizarse conforme a las necesidades de mantenimiento y compatibilidad del sistema.

Instalación
---Instalación del ambiente de desarrollo---
¿Cómo se instala el ambiente?
La implementación del sistema se llevará a cabo mediante la instalación directa de la aplicación en los dispositivos móviles de la empresa, así como a través de un proceso de capacitación dirigido a los usuarios finales.
La aplicación será distribuida en formato APK, el cual se instalará manualmente en los teléfonos Android asignados al personal.

---Ejecución de pruebas manuales---
¿Cómo ejecutar las pruebas manuales?
Las pruebas manuales del sistema se llevarán a cabo con el objetivo de validar el correcto funcionamiento de la aplicación en escenarios reales de uso. 
Estas pruebas serán realizadas directamente en los dispositivos móviles donde se instaló el aplicativo.
El proceso consiste en ejecutar casos de prueba previamente definidos, donde los usuarios o el equipo de pruebas realizarán acciones como:
Registro de nuevos productos en el inventario
Actualización de cantidades (entradas y salidas)
Consulta de productos disponibles
Verificación de sincronización de datos en tiempo real con Firebase
Validación del inicio de sesión y control de accesos
---Despliegue en ambiente local---
El sistema será desplegado directamente en los dispositivos móviles Android de la empresa mediante la instalación del archivo APK, permitiendo su uso inmediato por parte de los empleados.

---Despliegue en la nube (ej. Heroku)---

Por el momento, no se contempla un despliegue adicional en plataformas como Heroku u otros servicios similares, ya que la solución implementada utiliza Firebase como backend en la nube, el cual ya proporciona los servicios como base de datos en tiempo real.

CONFIGURACIÓN

Configuración del sistema

La configuración del sistema es realizada exclusivamente por la consultora Prime IT, encargada del desarrollo, implementación y puesta en marcha de la solución tecnológica.

El usuario final (Rodaclean) no tiene acceso a configuraciones internas del sistema, ya que estas son gestionadas de manera centralizada para garantizar la estabilidad, seguridad y correcto funcionamiento de la aplicación.

Entre las configuraciones realizadas por Prime IT se incluyen:

Definición del entorno (desarrollo, pruebas y producción)
Configuración de puertos y servicios del servidor
Gestión de variables de entorno
Parámetros generales del sistema

Configuración de dependencias
La configuración de los requerimientos técnicos necesarios para el funcionamiento del sistema, tales como:
Conexión a la base de datos
Integración con servicios externos
Configuración de servidores (aplicación, web, base de datos)
también es responsabilidad de Prime IT.

Uso
–Sección de referencia para usuario final–
El usuario final cuenta con acceso a las funciones operativas del sistema relacionadas con la consulta y actualización del inventario
Entre las principales acciones disponibles se encuentran:
Inicio de sesión mediante credenciales autorizadas
Consulta del inventario en tiempo real
Búsqueda y filtrado de productos
Registro de salida de productos vendidos
Consulta de reportes gráficos
Acceso al módulo de ayuda y soporte
El sistema está diseñado para ofrecer una interfaz intuitiva y de fácil uso para el personal operativo de Rodaclean
–Manual de administrador–
El administrador dispone de funcionalidades avanzadas para la gestión general del sistema y control del inventario.
Además de las funciones disponibles para el usuario final, el administrador puede:
Registrar nuevos productos
Actualizar existencias
Modificar información del inventario
Gestionar usuarios del sistema
Asignar permisos administrativos
Dar de baja usuarios
Supervisar reportes y estadísticas generales
Estas funciones permiten mantener el control operativo y administrativo del sistema de manera centralizada.
Contribución
Proposito
La presente sección define el proceso mediante el cual se gestionan las contribuciones al sistema, garantizando el control de cambios, la calidad del código y la estabilidad de la solución.
El desarrollo y mantenimiento del sistema es responsabilidad exclusiva de la consultora Prime IT.

 Clonar el repositorio
 Creación de ramas (branching)
 Envío de cambios (pull request)
 Proceso de revisión y merge
Politica de acceso al codigo
El código fuente del sistema es de tipo privado y cerrado, por lo que:
Los colaboradores de Rodaclean
Usuarios finales
Terceros o asociados
No tienen acceso ni permisos para modificar directamente el código fuente del sistema.
Esta política se implementa con el objetivo de:
Proteger la integridad del sistema
Mantener estándares de calidad
Evitar vulnerabilidades de seguridad
Sugerencias
Aunque no se permite la modificación directa del código, los colaboradores de Rodaclean y otros interesados pueden contribuir al mejoramiento del sistema mediante:
Reporte de errores
Propuestas de nuevas funcionalidades
Sugerencias de mejora en procesos
Estas contribuciones deberán realizarse a través de los canales oficiales de comunicación con Prime IT.
Una vez aprobados los cambios, estos serán integrados al sistema y desplegados en el entorno correspondiente por el equipo de Prime IT, asegurando su correcto funcionamiento antes de ser liberados a producción. 

ROADMAP
Estado actual del proyecto
Actualmente, el sistema cumple con los requerimientos y funcionalidades solicitadas por el cliente durante la fase de desarrollo e implementación.
Por el momento, no se tiene planeado agregar nuevas funcionalidades, módulos o cambios importantes a la aplicación, ya que la solución cubre las necesidades actuales de Rodaclean.

Solicitudes futuras
En caso de que el cliente requiera nuevas funcionalidades, mejoras o modificaciones en el futuro, estas podrán ser evaluadas e implementadas por la consultora Prime IT mediante nuevas fases de desarrollo.
Las posibles solicitudes futuras podrían incluir:
Nuevos módulos
Mejoras visuales
Integraciones externas
Reportes adicionales
Optimización de procesos
Todas las solicitudes estarán sujetas a evaluación técnica y aprobación por parte de ambas organizaciones.

Mantenimiento del sistema
Aunque actualmente no se contemplan nuevas funcionalidades, Prime IT continuará proporcionando soporte técnico y mantenimiento correctivo en caso de presentarse errores o incidencias dentro del sistema.
