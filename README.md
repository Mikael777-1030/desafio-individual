# Desafío Individual: Modelado EDO con Métodos Numéricos

**Asignatura:** Métodos Numéricos  
**Estudiante:** Brandon Mikael Quiñones Rosales  
**Fecha límite:** 6 de noviembre de 2026  

---

## 1. Descripción del Modelo y Contexto
Este proyecto implementa un modelo matemático basado en ecuaciones diferenciales ordinarias (EDO) de primer orden para resolver un problema real de la comunidad: **el monitoreo de la pérdida de la cadena de frío en biológicos (vacunas) ante fallas eléctricas en postas de salud comunitaria**.

* **Variable dependiente $T(t)$:** Temperatura interna del termo en grados Celsius [°C].
* **Variable independiente $t$:** Tiempo transcurrido en minutos [min].
* **Parámetros:** 
  * Temperatura ambiente ($T_m$) = $25\text{ °C}$
  * Constante de conductividad térmica ($k$) = $0.05\text{ min}^{-1}$
* **Condición inicial:** $T(0) = 4\text{ °C}$ (temperatura refrigerada inicial).

### Ecuación Diferencial (Ley de Enfriamiento de Newton):
$$\frac{dT}{dt} = -0.05(T - 25)$$

### Solución Analítica Exacta:
$$T(t) = 25 - 21e^{-0.05t}$$

---

## 2. Enlaces del Proyecto
* **Aplicación Web Interactiva (Simulador en línea):** [Enlace a tu GitHub Pages / Vercel]
* **Video Explicativo (1 minuto):** [Enlace a tu video de YouTube / Drive]

---

## 3. Métodos Numéricos Implementados
El simulador compara la solución analítica exacta frente a dos métodos numéricos utilizando idénticos parámetros y tamaño de paso $h$:
1. **Método de Heun (Runge-Kutta de 2.° Orden):** Predictor-corrector de orden intermedio.
2. **Método Clásico de Runge-Kutta de 4.° Orden (RK4):** Ponderación de cuatro pendientes para máxima precisión $O(h^5)$.

---

## 4. Instrucciones de Ejecución Local
Como la aplicación está desarrollada en **HTML, JavaScript puro y Chart.js** (sin servidores backend pesados), tienes dos formas de ejecutarla:

### Opción A: Directamente en tu navegador (Sin instalación)
1. Clona o descarga este repositorio en tu computadora.
2. Busca el archivo principal llamado `index.html`.
3. Haz doble clic sobre `index.html` para abrirlo en cualquier navegador web moderno (Chrome, Edge, Firefox).

### Opción B: Mediante Visual Studio Code (Live Server)
1. Abre la carpeta del repositorio en **Visual Studio Code**.
2. Asegúrate de tener instalada la extensión **Live Server**.
3. Haz clic derecho sobre el archivo `index.html` y selecciona **"Open with Live Server"**.
