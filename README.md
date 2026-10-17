# COMBATE Jinotega

Juego de pelea 2D para PC creado por Deyner Quiroz con IKEMEN GO, ambientado en Jinotega, Nicaragua.

## Versión 1.1.1

- Dificultad **Fácil, Medio y Difícil**, elegible en **Configuración → Dificultad** con izquierda/derecha. Elegí **Guardar y volver** para conservarla. También se respeta en la torre.
- La CPU regula pausas, defensa y combinaciones según la dificultad. Busca espacio para volver al centro y salir de las esquinas; el jugador conserva libertad de movimiento. La vida y el daño no aumentan con la dificultad.
- 17 luchadores, incluyendo Elian «Wanheda» y Lenn «El Tripas».
- 12 escenarios de Jinotega, incluyendo Avioneta, La Pelota, Calle La Salle, La Catedral, Lago de Apanás, Peñas Blancas, Cascada La Bujona e I.N.B.Z.
- Selección **Al azar**, torre de 10 rivales distintos, jugador contra CPU, jugador contra jugador y relevos 2vs2 con dos personajes por lado.
- Tres segmentos de energía: D requiere y consume 1000 (una barra); C requiere y consume 3000 (tres barras).

## Cómo actualizar

Cerrá el juego, abrí **COMBATE.exe** y elegí **Buscar actualizaciones**. Aceptá la versión **1.1.1** y, al terminar, elegí **Jugar**. Necesitás la instalación completa y el canal de actualizaciones configurado. Se puede actualizar directamente desde versiones anteriores.

El manifiesto latest.json está firmado. El lanzador comprueba firma y hashes, respalda los archivos que sustituye y conserva save/config.ini, incluyendo controles y audio.

## Controles de fábrica

P1: flechas; A/S ataques principales; Z/X ataques secundarios; D especial de una barra; C súper de tres barras; Enter provocación; Escape pausa. Para cubrirse, mantené la dirección contraria al rival. P2: I/J/K/L, R/T, F/G, Y/H y Shift derecho. Se pueden personalizar desde Configuración.

## Plataformas

Disponible actualmente para PC Windows. Android e iOS están en evaluación; todavía no hay versiones móviles publicadas ni fecha de lanzamiento.

## Validación

Pruebas del motor en Linux: carga de los 17 personajes, selección y persistencia de dificultad, movimiento de CPU e instalación firmada con conservación de configuración. Se conservan las animaciones y reglas de energía anteriores. La interfaz Windows y los mandos físicos no se ejecutaron en ese entorno.

Este repositorio distribuye actualizaciones de contenido; no contiene claves privadas ni una copia completa del motor.
