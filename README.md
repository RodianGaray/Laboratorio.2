# Laboratorio 2 — Coreographe y Librerías

Este laboratorio tiene como objetivo trabajar con el robot **Pepper** usando el entorno **Choreographe** y distintas librerías de Python para su programación.

## 1. Librerías

Se investigaron y ejemplificaron diferentes librerías usadas en la programación de Pepper:

- **qi**: Conexión entre Python y los servicios internos del robot (motores, voz, cámaras).
- **argparse**: Manejo de parámetros desde la línea de comandos.
- **sys**: Acceso a funciones del intérprete de Python.
- **os**: Interacción con archivos, directorios y sistema operativo.
- **almath**: Cálculos matemáticos para posiciones y trayectorias en 3D.
- **math**: Funciones matemáticas básicas (trigonometría, logaritmos, conversiones).
- **motion**: Control de articulaciones, posturas y movimientos.
- **httplib**: Comunicación con servidores y APIs externas.
- **json**: Manejo de datos en formato JSON.

---

## 2. Instalación de Choreographe, enlace con Pepper y generación de movimientos

1. Buscar y descargar **Choreographe 2.5**.  
2. Instalar desde el archivo `.tar.gz`.  
3. Ubicar la aplicación desde la terminal.  
4. Abrir Choreographe.  
5. Crear una secuencia de movimientos para Pepper con bloques visuales.  
6. Ejecutar la secuencia en el robot.  

---

## 3. Órdenes con Python

### 3.1 Conexión por SSH
- Conectarse al robot Pepper usando `ssh nao@<IP>`.

### 3.2 Creación de archivo Python
- Crear scripts directamente en el robot usando `nano hello_pepper.py`.

### 3.3 Ejemplo con **ALProxy**
- Uso de servicios como **ALTextToSpeech**, **ALMotion**, **ALRobotPosture** y **ALMemory** para controlar el robot.

### 3.4 Ejemplo con **qi.Application**
- Uso del framework moderno `qi` para crear sesiones y acceder a servicios con Python 3.

### 3.5 Ejecución del script
- Verificación de versiones (`python`, `python3`).  
- Ejecución con `python hello_pepper.py <IP>`.

### 3.6 Explicación de librerías
- Se repasaron las librerías utilizadas en los ejemplos: `naoqi.ALProxy`, `qi.Application`, `ALTextToSpeech`, `ALMotion`, `ALRobotPosture` y `ALMemory`.

---

## Autores
- **Rodian Daniel Garay Peralta**  
- **Mariana Lombana Rojas**

Docente: *Diego Alejandro Barragán Vargas*  
Universidad Santo Tomás  
5 de septiembre de 2025
