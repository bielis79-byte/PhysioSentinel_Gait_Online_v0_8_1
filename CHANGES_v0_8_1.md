# PhysioSentinel Gait Online v0.8.1

## Objetivo
Corregir la incoherencia interna detectada entre cadencia, CV, tiempo de apoyo y doble apoyo.

## Cambios
- Cadencia primaria calculada como 120 / duración media IC→IC de los mismos ciclos rectilíneos usados para stance/swing.
- CV calculado sobre esas mismas duraciones IC→IC.
- Los contactos bilaterales quedan como control secundario.
- Si la cadencia por contactos difiere >10% de la cadencia por ciclos, se suprime la asimetría temporal bilateral.
- El control recuento/cadencia usa la duración rectilínea utilizable y no la duración total con giro.
- Doble apoyo restringido al mismo dominio de ciclos válidos y contrastado con la ocupación de apoyo bilateral.
- Nuevas métricas de control: duración rectilínea utilizable, duración media IC→IC y discrepancia entre cadencia por ciclos y por contactos.
- Desfase tronco-pelvis normalizado circularmente al intervalo −180° a +180°.
- APP_VERSION corregida a 0.8.1-online.

## Alcance
Sigue siendo un análisis markerless 2D experimental. Los controles añadidos mejoran la coherencia matemática interna, pero no sustituyen plataforma de fuerzas ni análisis 3D instrumentado.
