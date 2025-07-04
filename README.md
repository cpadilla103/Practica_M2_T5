# Practica_M2_T5
# Burney Relief – Modelo 3D publicado

Este repositorio forma parte de la práctica del Tema 5 del Módulo 2 del curso de Digitalización del Patrimonio Cultural. El objetivo ha sido generar una malla optimizada con textura a partir de una nube de puntos, exportarla en formato X3D y publicarla en la web mediante GitHub Pages.

## 🖼️ Modelo seleccionado
**burney_relief_queen_of_the_night_draft**

Este modelo representa un bajorrelieve mesopotámico de la diosa Inanna/Ishtar, conocido como *Burney Relief* o *Queen of the Night*, datado en el segundo milenio a.C.
---

## Proceso de trabajo
1. **Triangulación**  
   Se realizó a partir de una nube de puntos densa mediante Poisson Reconstruction con una profundidad ajustada para evitar añadir vértices artificiales.

2. **Limpieza topológica**  
   Se eliminaron caras duplicadas, vértices no referenciados y elementos no manifold.

3. **Simplificación**  
   Se aplicó el filtro Quadric Edge Collapse Decimation, obteniendo un modelo con menos de 10.000 vértices.

4. **Parametrización UV**  
   Se realizó usando el filtro Voronoi Atlas, generando un mapa de coordenadas de textura eficiente y sin distorsiones importantes.

5. **Texturizado**  
   Se transfirió el color por vértice desde la nube de puntos original al modelo simplificado, generando una textura raster en resolución 1024x1024 px.

6. **Exportación y publicación**  
   El modelo fue exportado en formato `.x3d` con su textura asociada y publicado mediante X3DOM en GitHub Pages.
---

## Licencia

El modelo original fue procesado con fines exclusivamente académicos. Cualquier reutilización queda sujeta a los términos del curso y a la propiedad intelectual del modelo base.

