# Control por Torque Computado de un Robot Manipulador RR

Este repositorio contiene el modelado matemático, la simulación y la documentación de una estrategia de control no lineal para un brazo robótico de dos grados de libertad (configuración RR) operando en el plano vertical. 

Proyecto desarrollado para la materia de *Seminario de Problemas de Modelado y Simulación de Sistemas* en el Centro Universitario de Ciencias Exactas e Ingenierías (CUCEI).

## Descripción del Proyecto

El objetivo de esta práctica es garantizar que el efector final del robot siga con precisión una trayectoria circular en el espacio cartesiano. Para lograrlo, el proyecto se divide en:
* **Modelado Dinámico:** Obtención de las matrices de inercia, Coriolis y gravedad mediante el formalismo de Euler-Lagrange.
* **Cinemática Inversa:** Transformación de la trayectoria cartesiana a referencias articulares.
* **Control:** Implementación de una ley de control por Torque Computado con acción Proporcional-Derivativa (PD) para linealizar la dinámica del sistema y anular el error en estado estacionario.

## Estructura del Repositorio

* `/Simulacion`: Contiene los archivos de MATLAB y Simulink.
* `/Documentacion`: Contiene el reporte técnico final en formato PDF, el código fuente en LaTeX y las gráficas de validación.

## Requisitos de Software

* MATLAB 
* Simulink

## Instrucciones de Uso

Para replicar la simulación en tu equipo local, sigue estos pasos:

1. Clona este repositorio o descarga los archivos de la carpeta `Simulacion`.
2. Abre MATLAB y navega hasta el directorio de la simulación.
3. Ejecuta primero el script de inicialización para cargar los parámetros físicos y las ganancias del controlador en el Workspace:
   ```matlab
   run('init.m')
