# Reflexión del Taller: Sistema Saludador

## 1. Retos y Dificultades Técnicas

El desarrollo de este laboratorio representó un desafío técnico significativo, mucho más allá de la simple escritura de código. El primer gran obstáculo fue la configuración del entorno. Inicialmente intenté trabajar en mi partición de Linux, pero me encontré con problemas de seguridad al instalar paquetes .deb (errores de sandbox) y fallos de compatibilidad gráfica con la arquitectura al intentar forzar la ejecución (--disable-gpu). A esto se sumó la falta de espacio en disco para usar alternativas como AppImage, lo que me obligó a migrar todo mi entorno de trabajo a Windows para poder continuar.

Adicionalmente, enfrentarme a Cursor IDE por primera vez fue abrumador. Si bien es una herramienta poderosa, al principio la IA generaba archivos y configuraciones automáticas (como las carpetas .vscode, los archivos mvnw o .gitignore) que yo no comprendía. Tomé la decisión de pausar la automatización para entender primero qué estaba haciendo la máquina antes de delegarle el trabajo.

## 2. Descubrimientos y Sorpresas

El mayor descubrimiento fue entender la verdadera función de Maven. Al principio creía que JavaFX era un compilador y Maven un instalador de Java. Investigando y preguntando, descubrí que Maven es en realidad un gestor de proyectos que se encarga de ir a internet y descargar las "piezas" gráficas (librerías de JavaFX) que mi código necesita, ya que estas dejaron de venir incluidas por defecto en las versiones modernas de Java.

También me sorprendió gratamente lo intuitivo que es el código de JavaFX una vez se entiende su estructura. Usar contenedores como VBox para apilar elementos verticalmente hizo que el diseño de la interfaz fuera muy lógico y ordenado, similar a armar bloques de construcción.

## 3. Comandos y Estructuras Clave

Durante este proyecto, interioricé varios conceptos nuevos:

- `mvn clean javafx:run`: El comando vital para limpiar construcciones previas, compilar el código actual y lanzar la ventana gráfica en un solo paso.
- Componentes de JavaFX: Entendí la diferencia entre un `Label` (texto estático para instrucciones o resultados), un `TextField` (caja de entrada de datos) y un `Button` (el detonante de las acciones).
- `.setOnAction(...)`: La función que le da vida al botón, permitiendo capturar eventos y ejecutar la lógica de concatenación de texto para generar el saludo final.

## Conclusión

Este laboratorio me enseñó que en el desarrollo de software, la escritura de código es solo una parte del proceso. La configuración del entorno, la resolución de problemas de compatibilidad del sistema operativo y la comprensión profunda de las herramientas (como Maven y Cursor) son habilidades fundamentales para que un proyecto llegue a buen término.
