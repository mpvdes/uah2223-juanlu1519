# Charla Daniel Mery

La charla se dividió en dos grandes apartados: explicación de un sistema operativo y todo lo que compone y, por otro lado, un repaso de lo que es el software libre.

## ¿Qué es un sistema operativo?

Es un programa que maneja recursos y suminista abstracciones. También se entiende como un conjunto de programas que gestiona los recursos de hardware y provee servicios a las aplicaciones de software. Comienza a trabajar cuando se enciende el ordenador y gestiona el hardware desde los niveles más básicos, permitiendo también la interacción del usuario.

Uno de sus propósitos es gestionar los recursos, localizar y proteger el acceso al hardware.

### Funciones del sistema operativo

- Gestión de procesos: crear, destruir, suspender, reanudar, sincronizar y comunicar procesos.

- Gestión de memoria: almacenamiento de procesos, asignar y liberar memoria, decidir cuanta memoria se asigna a un proceso y controlar las partes de la memoria que se están utilizando.

- Gestión de archivos: lo hace mediante el "file system", que es un conjunto de normas y procedimientos para almacenar información en dichos dispositivos.

- Gestión de I/O: se encarga de capturar interrupciones, enviar y manejar datos en memoria que recoge desde los dispositivos.

### ¿Qué es un sistema de computo?

Está formado por:

- Hardware: es todo lo tangible, como el CPU y periféricos (teclado, ratón, memorias, etc.).

- Software: todo lo intangible, como lenguajes de programación, sistemas operativos y software de aplicación.

Entre el hardware y software encontramos lo que llamamos firmware. Se encarga de comprobar que haya un hardware básico para poder trabajar el software.

- Humanware: desarrolladores, administradores y usuarios finales.

#### Hardware

- CPU: mononúcleo o multinúcleo.

- Periféricos: entrada, mixtos o de salida.

#### Software

- Lenguajes de programación

- Sistemas operativos

- Programas aplicaciones

### ¿Qué tareas realizamos con un computador?

Con un ordenador podemos realizar varias tareas como son: edición de texto, imagen, sonido y vídeo; comunicaciones (VoIP); Internet ; Videojuegos; aplicaciones de nicho y generales.

### Kernel

Un kernel es un software que forma una capa entre el hardware y el sistema operativo. Es el primer programa que se carga en el inicio del sistema. Gestiona recursos de memoria, de CPU y todos los procesos en cualquier computador. Tofdas las solicitudes a otros recursos pasan por el núcleo. Por ejemplo, si queremos imprimir, la instrucción de impresión se procesa a través del núcleo.

Es el corazón del sistema operativo pero por sí solo no hace nada, necesita hardware, software y humanware.

Hay diferentes tipos de kernel:

- Kernel monolítico: Windows, iOS, Linux...

- Micro Kernel: Hurd, Minix, Redox...

Ambas tienen sus ventajas y desventajas. El tipo de núcleo debe seleccionarse en función de las necesidades y los requisitos que deben cumplir.

### Puntos para reflexionar

- Futuro y presente de Rust

- ¿Es Redoz actualmente un SO de producción?

- ¿Los microkernel son una tendencia posible?

- ¿Son Risc V y ARM un camino inevitable?

- ¿El grafeno logrará sustituir al silicio?

- La importancia del ahorro energético

- ¿El tamaño del chip importa?

## Historia del software libre

Hay varias confusiones y malentendidos. Open Source no es lo mismo que Software Libre al igual que Software Libre no es Linux. Mucha gente que Stallman y Torvalds fueron quienes crearon el Software Libre. Sin embargo hay varios desarrolladores que trabajaron en ello. También hay quien piensa que Software libre significa gratis, pero en realidad significa libertad para copiar, utilizar, modificar, crear, etc.

Hay grandes comparaciones entre el mundo antiguo y la edad contemporánea hablando de software libre, desde los filósofos, pasando por los científicos hasta llegar a los hackers.

### ¿Qué es el Software Libre?

Es mucho más que un kernel, programa o sistema operativo. Es una filosofía y una actitud frente a la manera de resolver problemas de cualquier orden, o sea, un proceso de desarrollo integral.

Internet y el mundo interconectado en el que vivimos hoy, no sería posible sin el grandioso aporte del Software Libre. Está presente en Mac, Play Station 4, Nintendo, iPhone, Android, etc.

El software libre también está presente en una de las grandes revoluciones del siglo XXI: el blockchain. Esta es una tecnología de software libre que no hay que confundir con Bitcoin.

### Características del Software Libre

Cuatro libertades esenciales:

- Libertad de uso

- Libertad de estudio

- Libertad de distribución

- Libertad para modificar

Otras facetas importantes son: compartir el conocimiento, público y de fácil acceso, alentar el trabajo en comunidades, difusión del conocimiento, crecimiento rápido y diverso, sustituir la competencia por la colaboratividad y disminuir la brecha social y regional.

Resumidamente: libertad, diversidad y oportunidad.

### Tipos de licencias Open Source

- Copyleft

- BSD y MIT

- Creative Commons

#### Dilema cajas negras

No son auditables desde el punto de vista de seguridad, no permiten compartir el conocimiento y no hay control del programa por parte del usuario. En definitiva, no sirven para la educación ni para la seguridad.
