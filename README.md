# Sistema Saludador - Taller de JavaFX

Este proyecto es una aplicación de escritorio desarrollada en Java utilizando la librería gráfica JavaFX y gestionada a través de Maven. Fue creado como parte del taller universitario para demostrar el manejo de interfaces gráficas básicas y el uso de herramientas asistidas por IA (Cursor IDE).

## Descripción del Proyecto

El "Sistema Saludador" despliega una ventana interactiva que le solicita al usuario tres datos:

- Nombre
- Edad
- Hora (AM/PM)

Al hacer clic en el botón "Solicitar saludo", el sistema procesa la información y devuelve un mensaje personalizado en la pantalla.

## Requisitos Previos

Para ejecutar este proyecto en tu máquina, necesitas tener instalado:

- **Java Development Kit (JDK)**: Versión 17 o superior (el proyecto está configurado para la versión 21).
- **Maven**: (Opcional, ya que el proyecto incluye los scripts de Maven Wrapper `mvnw` y `mvnw.cmd`).

## Instrucciones de Ejecución

Sigue estos pasos para compilar y ejecutar la aplicación:

### 1. Clonar o descargar el repositorio

Abre una terminal y ubícate en la carpeta raíz del proyecto (donde se encuentra el archivo `pom.xml`).

### 2. Ejecutar mediante Maven

En la terminal integrada de tu IDE (como Cursor o VS Code) o en la consola del sistema, ejecuta el siguiente comando:

```bash
mvn clean javafx:run
```

### 3. Usando los scripts (Alternativa)

Si estás en Windows y prefieres usar los scripts incluidos, puedes ejecutar:

```bash
.\mvnw.cmd clean javafx:run
```

> **Nota**: También se incluye un archivo `run.bat` configurado localmente para arrancar la aplicación de forma directa.

## Estructura de Entregables

```text
├── src/main/java/
│   └── SistemaSaludador.java    # Código fuente de la aplicación
├── pom.xml                       # Configuración de dependencias de Maven
├── docs/prompts/                 # Historial de interacción con la IA (Cursor)
├── Reflexion.md                  # Documento de análisis y aprendizajes
├── README.md                     # Este archivo
├── run.bat                       # Script para ejecución directa (Windows)
└── documentacion.md             # Documentación general del laboratorio
```

## Documentación Adicional

- [Documentación del Laboratorio](documentacion.md) - Información adicional sobre el proyecto
- [Reflexión](Reflexion.md) - Análisis sobre los retos y aprendizajes del taller

---

*Proyecto desarrollado como parte del curso de Ingeniería de Software - Octubre 2026*
