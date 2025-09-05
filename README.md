# Laboratorio 2 — Choreographe y Librerías

Este laboratorio tiene como objetivo trabajar con el robot **Pepper** usando el entorno **Choreographe** y distintas librerías de Python para su programación.

---

## 1. Librerías

A continuación, se detallan las librerías investigadas y sus funciones principales en la programación de Pepper:

### Librería qi
La librería **qi** es la base del framework NAOqi. Se encarga de la conexión entre los programas en Python y los servicios internos del robot, tales como control de motores, síntesis de voz, cámaras, micrófonos y sensores táctiles.  
**Funciones principales:**
- Crear sesiones y conectarse al robot mediante IP y puerto.  
- Acceder a servicios como ALMotion, ALTextToSpeech o ALMemory.  
- Publicar y suscribirse a eventos internos (ejemplo: sensores táctiles).  

### Librería argparse
La librería **argparse** permite gestionar argumentos desde la línea de comandos. Es útil para ejecutar scripts en Pepper sin modificar el código fuente cada vez.  
**Funciones principales:**
- Definir parámetros opcionales y obligatorios.  
- Validar automáticamente los tipos de datos.  
- Mostrar ayuda interactiva con --help.  

### Librería sys
La librería **sys** permite acceder a funciones del intérprete de Python. En Pepper se usa para gestionar la ejecución de scripts y cargar rutas de módulos externas.  
**Funciones principales:**
- Finalizar programas con sys.exit().  
- Obtener parámetros con sys.argv.  
- Modificar rutas de búsqueda con sys.path.  

### Librería os
La librería **os** permite interactuar con el sistema operativo. En Pepper se utiliza para manejar archivos, directorios y ejecutar comandos del sistema.  
**Funciones principales:**
- Crear y eliminar carpetas.  
- Ejecutar comandos del sistema.  
- Gestionar rutas y variables de entorno.  

### Librería almath
La librería **almath** fue desarrollada por Aldebaran Robotics. Proporciona herramientas matemáticas para trabajar con transformaciones, posiciones y rotaciones en 3D.  
**Funciones principales:**
- Cálculo de ángulos y distancias en 3D.  
- Manejo de cuaterniones y matrices.  
- Soporte para cálculos de trayectorias.  

### Librería math
La librería **math** incluye funciones matemáticas básicas y avanzadas, siendo útil para cálculos relacionados con el movimiento del robot.  
**Funciones principales:**
- Funciones trigonométricas (seno, coseno, tangente).  
- Exponenciales y logaritmos.  
- Conversión de grados a radianes.  

### Librería motion
La librería **motion** es una de las más importantes en Pepper, ya que gestiona los movimientos del robot.  
**Funciones principales:**
- Controlar articulaciones y ángulos.  
- Gestionar posturas y equilibrio.  
- Ejecutar animaciones y desplazamientos.  

### Librería httplib
La librería **httplib** (en Python 3 se reemplaza por http.client) permite que Pepper se comunique con servidores web o APIs externas.  
**Funciones principales:**
- Realizar solicitudes GET y POST.  
- Enviar y recibir datos desde servidores web.  
- Acceder a información de APIs en tiempo real.  

### Librería json
La librería **json** permite trabajar con datos en formato JSON, muy útil para intercambio de información estructurada.  
**Funciones principales:**
- Convertir objetos de Python a JSON.  
- Decodificar JSON a objetos de Python.  
- Intercambiar datos con servicios web.  

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

