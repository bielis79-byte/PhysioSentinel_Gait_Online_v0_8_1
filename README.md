---
title: Sentinel Gait
emoji: 🚶
colorFrom: blue
colorTo: green
sdk: docker
app_port: 7860
pinned: false
---

# PhysioSentinel Gait Online v0.8.1

Versión centrada en mejorar la coherencia biomecánica de las métricas temporales 2D.

Principales cambios: exclusión automática de giro/transiciones, CV y asimetría derivados de contactos
I/D validados, doble apoyo restringido a ciclos válidos y controles internos que suprimen resultados
incoherentes en lugar de mostrarlos como fiables.

Las métricas markerless 2D son experimentales y deben integrarse con la observación clínica.
