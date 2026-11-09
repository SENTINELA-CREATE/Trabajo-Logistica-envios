Hola :) Este es el trabajo Numero 2 de el profesor WAZ la fk cabra



Edición numero 2 de el read me. para el 3 commit. estoy avanzando en el trabajo de jarvis. cuando lo termine me comunicare con Waz para mostrárselo







Jarvis ya cuenta con una base funcional de asistente local para Windows, con procesamiento mediante Ollama, interfaz gráfica, memoria y un sistema de herramientas con controles de seguridad.

1\. Base del sistema

\- Proyecto configurado en Windows con Python 3.14.4.

\- Arquitectura híbrida diseñada con prioridad local.

\- Ollama funcionando como motor principal, usando qwen2.5:3b.

\- Reglas de coste cero y privacidad local: ZERO\_COST\_ONLY=True y local\_only=True.

\- Conexiones de pago y servicios remotos deshabilitados.

2\. Interfaz gráfica

\- Interfaz desarrollada con Tkinter.

\- Tema oscuro Catppuccin Mocha.

\- Generación de respuestas en segundo plano para evitar bloquear la ventana.

\- Ventana de ajustes y privacidad independiente.

\- Botón de micrófono preparado para las funciones de voz.

3\. Sistema de voz

\- Hito 4A completado: infraestructura básica de audio local.

\- Grabación temporal en memoria RAM, sin guardar audio en disco.

\- Reproducción de audio y control de interrupciones.

\- Integración con la voz nativa de Windows mediante SAPI5.

\- Hito 4B: plan técnico de Piper TTS revisado.

\- La implementación de Piper todavía no está confirmada como completada.

4\. Memoria y herramientas

\- Sistema de almacenamiento con SQLite.

\- Sistema de auditoría y autorización mediante tokens HMAC.

\- Herramientas de escritura de archivos:

  - fs.write(action="create").

  - fs.write(action="overwrite").

\- Herramientas de eliminación reversible:

  - fs.delete.

  - fs.restore.

\- Sistema de cuarentena para evitar la eliminación física definitiva de archivos.

\- Recuperación ante interrupciones y verificaciones de integridad.

5\. Seguridad

\- Restricciones para proteger archivos personales y del sistema.

\- Bloqueos frente a rutas peligrosas y enlaces simbólicos.

\- Verificación de identidad física de archivos mediante File ID, volumen y SHA-256.

\- Protección frente a operaciones simultáneas.

\- Registro de operaciones y recuperación controlada.

\- Las operaciones sensibles requieren autorización explícita.

6\. Pruebas y validación

Área	Último resultado reportado

Hito 3D.1B, escritura y sobrescritura	41/41

Regresión 3D.1A y 3D.2	135/135

Suite completa	790 aprobadas

Pruebas omitidas	1

Pruebas fallidas	0



Resultados según el último informe de Antigravity. El cierre formal de 3D.1B quedó pendiente de aclarar tres puntos de auditoría.



Estado general

Base del asistente

Funcional



Interfaz gráfica

Implementada



Voz local básica

Hito 4A completado



Herramientas de archivos

Auditoría pendiente de cierre



Voz avanzada con Piper

Pendiente



Skills y funciones adicionales

Para etapas posteriores





En pocas palabras: ya construimos los cimientos de Jarvis: un asistente local que puede conversar, tiene interfaz gráfica, memoria, infraestructura de voz y herramientas para gestionar archivos con controles de seguridad.



Todavía queda trabajo para convertirlo en el asistente completo que imaginamos. La prioridad es terminar y validar las funciones fundamentales antes de añadir capacidades adicionales.

