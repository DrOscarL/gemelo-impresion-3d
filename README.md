# Gemelo de impresión 3D · Construcción 5.0

Demo 3D interactiva creada para la charla **"Construcción 5.0: Gemelos Virtuales, Inteligencia Artificial, Sistemas Ciberfísicos y Manufactura Aditiva"** (Feria TAC 2026, 19 de octubre de 2026).

Una impresora de hormigón tipo pórtico imprime un muro de 40 capas sobre la silueta de su modelo BIM. Un escáner mide el ancho de cada capa y el gemelo digital recorre la escala de madurez de la charla:

| Peldaño | Qué ocurre en la demo |
|---|---|
| Representar | El modelo de diseño (BIM) se muestra como silueta celeste. |
| Observar | El escáner láser mide el ancho de cada capa. |
| Predecir | Ante un desvío, el gemelo proyecta en qué capa saldrá de tolerancia (±5 %). |
| Optimizar | Calcula la nueva velocidad del robot para recuperar los 50 mm de diseño. |
| Actuar | Aplica el ajuste al robot desde la capa siguiente (lazo cerrado). |

**Ver la demo:** https://droscarl.github.io/gemelo-impresion-3d/

## Controles

| Tecla | Acción |
|---|---|
| Espacio | Comenzar / pausar |
| R | Reiniciar |
| G | Alternar vista Obra / Gemelo |
| L | Lazo cerrado / abierto |
| D | Perturbar o normalizar la mezcla |
| 1, 2, 4 | Velocidad de la simulación |
| F | Pantalla completa |

Arrastra para orbitar la cámara y usa la rueda para acercar.

## Uso sin internet

`index.html` es autocontenido: incluye three.js y funciona con doble clic, sin conexión. Las tipografías se cargan desde Google Fonts cuando hay internet; sin conexión se usa la fuente del sistema.

## Nota

Es una simulación didáctica. El modelo de proceso (ancho del cordón proporcional a caudal/velocidad, con una perturbación de fluidez de la mezcla) está simplificado para ilustrar el concepto de gemelo digital en lazo cerrado; no representa una impresora ni una mezcla específicas.

## Autoría y créditos

- Dr. Oscar Loyola V. · Grupo de Sistemas Ciber-Físicos Inteligentes (GSCFI) · Universidad de Las Américas
- Gráficos 3D con [three.js](https://threejs.org) r128 (licencia MIT), incluido en `index.html`.
