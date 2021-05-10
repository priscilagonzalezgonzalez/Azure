## INTRODUCCIÓN A LOS ASPECTOS BÁSICOS DE AZURE

#### Cloud computing
La informática en la nube o cloud computing ofrece servicios informáticos a través de internet (o la nube). Ejemplos de servicios que ofrece: servidores, almacenamiento, bases de datos, redes, software, análisis e inteligencia.

#### Cloud provider
El proveedor de nube te permite elegir las características que deseas para tu software. Los servicios y características que ofrecen dependen del proveedor, pero las más comunes son velocidad de procesamiento y espacio de almacenamiento. Solo pagas por el servicio que estás utilizando. El proveedor se encarga de mantener la infraestructura solicitada. 

#### Confiabilidad 
Las aplicaciones basadas en la nube proporcionan una experiencia de usuario continua sin tiempo de inactividad perceptible aunque ocurran errores. 

#### Escalabilidad
**Vertical**: La capacidad aumenta agregando RAM o procesamiento adicional.
**Horizontal**: La capacidad aumenta agregando más instancias. 

#### Elasticidad
La necesidad de recursos se confugura de forma automática.

#### Agilidad
La configuración e implementación de recursos conforme cambian los requisitos de la aplicación es rápida.

#### Distribución geográfica
Los centros de datos están ubicados en distintas regiones del mundo. Las aplicaciones pueden ser implementadas en distintas regiones.

#### Recuperación ante desastres
Los recursos basados en la nube utilizan copias de seguridad distribuidas en los distintos centros de datos para proteger los datos en casos de desastre.

#### Modelo de servicio 
Definen los distintos niveles de responsabilidad compartidad entre un proveedor y el cliente (o quien adquiere los servicios).

#### IaaS
Modelo de servicio en la nube. El proveedor de servicios mantiene actualizado el hardware, pero el mantenimiento del sistema operativo y la configuración de red no es su responsabilidad.

#### PaaS
Modelo de servicio en la nube. El proveedor de servicios administra las máquinas virtuales y los recursos de red, pero el inquilino implementa sus aplicaciones en el entorno seleccionado.

#### SaaS
Modelo de servicio en la nube. El proveedor de servicios administra todos los aspectos del entorno de la aplicación, máquinas virtuales, recursos de red, almacenamiento de datos y aplicaciones. Solo es necesario proporcionar los datos de la información.

![Modelos de servicio en la nube](modelo.png)

#### Informática sin servidor
El término procede del hecho de que las tareas asociadas a la administración de la infraestructura son invisibles para el desarrollador. La informática sin servidor permite que las organizaciones optimicen mejor los recursos y se centren en la innovación.

#### Nube pública
Los servicios son ofrecidos a través de internet y son públicos para quien quiera comprarlos. Los recursos (almacenamiento, servidores) son propiedad de un proveedor de servicios.

#### Nube privada
Los recursos informáticos están disponibles para el uso único de la organización propietaria. Esto no quiere decir que la nube privada esté ubicada en un centro de datos local de la organización sino que puede ser hospedada en un proveedor de servicios de nube.

#### Nube híbrida
Combina ambas nubes (privada y pública). Es posible compartir datos y aplicaciones entre ellas. 

#### Azure
Azure ofrece servicios en la nube, por ejemplo, ejecutar las aplicaciones existentes en máquinas virtuales, bots inteligentes, aprendizaje automático, etc.

#### Virtualización
La vitualización permite particionar un equipo o servidor físico en varias máquinas virtuales. Cada máquina virtual opera de forma independiente, pueden utilizar diferentes sistemas operativos mientras comparten los recursos de una sola máquina.

#### Hipervisor
Un hipervisor permite que un ordenador preste soporte a varias máquinas virtuales, mediante el uso compartido de recursos como la memoria y el procesamiento.
**Hipervisor tipo 1:** Se ejecuta directamente en el hardware del host.
**Hipervisor tipo 2:** Se ejecutan como una capa de software sobre un sistema operativo, como otro programa informático. Como VMware Workstation.

#### API
Application Programming Interfaces. Permite la comunicación entre dos aplicaciones de software a través de un conjunto de reglas. Ejemplos: 
- Cuando abres un juego para móvil y puedes iniciar sesión con la cuenta de Facebook.
- Cuando una aplicación te manda notificaciones al móvil.

#### API REST
Una API REST usa HTTP. Define un conjunto de funciones que los desarrolladores pueden realizar: solicitudes y recibir respuestas a través del protocolo HTTP, como GET y POST.

#### Fabric Controller
**Fabrics:** Son un grupo de máquinas en un centro de datos conectadas a un switch. A este grupo se le llama *cluster*. 
Cada cluster es administrado por un *fabric controller*. 
**Tareas del Fabric Controller**
- Administra la asignación de recursos para una aplicación específica.
- Monitorea la salud el servicio de almacenamiento y computo.
- Recuperación de fallas para un sistema.
- Cuando una máquina virtual falla, una nueva es asignaba por el *fabric controller*.
Por lo tantom todas las tareas inteligentes son realizadas por el *fabric controller*.

#### Orquestación de servicios
La orquestación de servicios es la configuración, gestión y coordinación automatizadas de los sistemas informáticos, las aplicaciones y los servicios. Es responsable de responder a peticiones de usuario.

#### Centro de datos
![Imagen animada de un centro de datos](centro_datos.jpg)
Un centro de datos tiene un conjunto de estantes llenos de servidores y cada servidor tiene un hipervisor para correr múltiples máquinas virtuales. Un switch de red provee conectividad a todos esos servidores. Cada uno de los servidores cuenta con un *fabric controller*, el cual está conectado al orquestador.
Por ejemplo, el usuario hace una petición, desde la interfaz del Portal web de Azure, de crear una máquina virtual. El orquestador empaqueta lo necesario, elige la estantería de servicios más adecuada y manda la petición al *fabric controller*, el cual crea la máquina virtual y finalmente, el usuario obtiene su máquina virtual.

