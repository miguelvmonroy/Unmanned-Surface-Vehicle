# Autonomous Boat – Autonomous Navigation Project

<img width="1144" height="485" alt="image" src="https://github.com/user-attachments/assets/a34d9b2f-c372-44f5-8eae-c62da3be81b7" />

![Project Status](https://img.shields.io/badge/Estado-En%20Desarrollo-yellow)
![Versión](https://img.shields.io/badge/Versión-1.0.0-blue)
![License](https://img.shields.io/badge/Licencia-MIT-green)
![ROS 2](https://img.shields.io/badge/ROS%202-Jazzy-brightgreen)
![Gazebo](https://img.shields.io/badge/Gazebo-Harmonic-orange)

---

# 🔬 Documentación

> **ES:** Bienvenido a la documentación técnica del proyecto de investigación de **navegación autónoma de un USV** (Unmanned Surface Vehicle — vehículo de superficie no tripulado).
>
> **EN:** Welcome to the technical documentation of the research project on **autonomous navigation of a USV** (Unmanned Surface Vehicle).

---

## 🎯 Objetivo del proyecto / Project Goal

### 🇪🇸 Español

Desarrollar un **control + trayectoria** para una embarcación autónoma que navegue de forma segura en aguas con perturbaciones marinas (olas, corrientes y viento), validado primero en simulación y luego desplegado en hardware real.

**¿Qué significa esto en palabras simples?**

- La embarcación debe **llegar sola** de un punto A a un punto B.
- Debe **corregir su rumbo** si las olas o el viento la desvían.
- Debe **detenerse de forma segura** al llegar.
- Todo el comportamiento se prueba primero en un **simulador 3D** antes de construir el barco físico.

### 🇬🇧 English

Develop a **control + trajectory** system for an autonomous boat that navigates safely in waters with marine disturbances (waves, currents, and wind), validated first in simulation and then deployed on real hardware.

**What does this mean in plain words?**

- The boat must **reach point B from point A on its own**.
- It must **correct its heading** if waves or wind push it off course.
- It must **stop safely** upon arrival.
- All behavior is tested first in a **3D simulator** before building the physical boat.

---

## 🚤 ¿Qué se ha logrado hasta ahora? / What has been achieved so far?

### 🇪🇸 Español

| Logro | Estado |
|---|---|
| Simulación del barco en un entorno marino 3D | ✅ Completado |
| Control manual del barco desde teclado | ✅ Completado |
| Lectura de sensores en tiempo real | ✅ Completado |
| Navegación autónoma de A→B | 🔄 En progreso (40%) |
| Pruebas en hardware real | ⏳ Pendiente |

**En palabras simples:** ya puedo controlar el barco virtual, leer sus sensores y hacer que navegue solo hacia un destino. El siguiente paso es que lo haga de forma **robusta** ante olas y corrientes, y luego construir el barco físico.

### 🇬🇧 English

| Milestone | Status |
|---|---|
| Boat simulation in a 3D marine environment | ✅ Completed |
| Manual keyboard control of the boat | ✅ Completed |
| Real-time sensor reading | ✅ Completed |
| Autonomous A→B navigation | 🔄 In progress (40%) |
| Real hardware testing | ⏳ Pending |

**In plain words:** I can already control the virtual boat, read its sensors, and make it navigate on its own toward a destination. The next step is making it **robust** against waves and currents, and then building the physical boat.

---

## 🧭 ¿Cómo funciona la navegación autónoma? / How does autonomous navigation work?

### 🇪🇸 Español

El sistema funciona en tres capas:

1. **Percepción** — El barco lee su posición y orientación desde el simulador.
2. **Decisión** — Un controlador calcula cuánta potencia dar a cada motor para acercarse al destino.
3. **Acción** — Los motores reciben la orden y el barco se mueve.

**Control + Trayectoria** combina dos ideas:

- **Control:** mantener el barco estable y corregir desviaciones.
- **Trayectoria:** planificar el camino más seguro y eficiente hacia el destino.

### 🇬🇧 English

The system works in three layers:

1. **Perception** — The boat reads its position and orientation from the simulator.
2. **Decision** — A controller calculates how much power to send to each motor to approach the destination.
3. **Action** — The motors receive the command and the boat moves.

**Control + Trajectory** combines two ideas:

- **Control:** keep the boat stable and correct deviations.
- **Trajectory:** plan the safest and most efficient path to the destination.

---

## 📚 Secciones / Sections

Usa el menú superior para navegar por la documentación:

| Sección | Descripción / Description |
|---|---|
| **🚤 Autonomous Boat** | Descripción general del proyecto USV / USV project overview |
| **🎮 Boat Control** | Control manual del WAM-V en VRX / Manual WAM-V control in VRX |
| **🧭 Autonomous Navigation** | Navegación autónoma A→B / Autonomous A→B navigation |
| **🎯 Pure Proportional Controller** | Análisis del controlador P / P controller analysis |
| **📊 Visualizer v6** | Visualizador de trayectoria en RViz2 / Trajectory visualizer in RViz2 |
| **🔧 Installation Guide** | Guía de instalación / Installation guide |
| **💻 Native Ubuntu Setup** | Configuración del hardware / Hardware setup |
| **⚙️ WSL2 Setup** | Entorno WSL2 + ROS 2 + Gazebo / WSL2 + ROS 2 + Gazebo environment |
| **🚀 GPU Acceleration** | Aceleración por GPU / GPU acceleration |
| **🖥️ Complete System** | Cómo lanzar el sistema completo / How to launch the complete system |

---

## 🛠️ Tecnologías / Technologies

| Tecnología | Propósito / Purpose |
|---|---|
| **ROS 2 Jazzy** | Middleware de robótica / Robotics middleware |
| **Gazebo Harmonic** | Simulador 3D / 3D simulator |
| **VRX** | Simulador de embarcaciones / USV simulator |
| **Python 3.12** | Scripts de control / Control scripts |
| **C++ 17** | Nodos ROS 2 / ROS 2 nodes |

---

## 🎓 ¿Por qué es importante este proyecto? / Why does this project matter?

### 🇪🇸 Español

- **Investigación aplicada:** combina teoría de control, simulación y robótica real.
- **Impacto ambiental:** los USV pueden monitorear océanos, ríos y puertos sin tripulación.
- **Formación:** documenta paso a paso cómo construir un barco autónomo desde cero.
- **Código abierto:** todo el proyecto está disponible en GitHub para que otros lo repliquen.

### 🇬🇧 English

- **Applied research:** combines control theory, simulation, and real robotics.
- **Environmental impact:** USVs can monitor oceans, rivers, and ports without a crew.
- **Education:** documents step by step how to build an autonomous boat from scratch.
- **Open source:** the entire project is available on GitHub for others to replicate.

---

⭐ **ES:** Si te gusta este proyecto, ¡no olvides darle una estrella en GitHub!
⭐ **EN:** If you like this project, don't forget to star it on GitHub!

---

*Última actualización / Last update: Octubre 2026 / October 2026*

⭐ If you like this project, don't forget to give it a star on GitHub!

⭐ Si te gusta este proyecto, ¡no olvides darle una estrella en GitHub!
