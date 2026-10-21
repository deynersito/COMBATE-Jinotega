# COMBATE Jinotega

Juego de pelea 2D para PC creado por Deyner Quiroz con IKEMEN GO, ambientado en Jinotega, Nicaragua.

## Versión 1.1.6

- Agrega **El Poli**: ataques con amansa bolos, multas voladoras y frase de victoria **«Son 500»**. Disponible en selección, versus y Torre Arcade, con sus retratos.
- Agrega los escenarios **El Mural** y **La Turbina**. El plantel cuenta con **22 personajes y 14 escenarios**.
- Conserva todo el contenido de 1.1.5, incluido el arreglo del actualizador y los ajustes personales de controles y audio.

### Correcciones de 1.1.5 que se conservan

- Corrige el error **«tipo de archivo no permitido»** al buscar actualizaciones. Las listas de movimientos de Ector, Héctor, El Conejo y El Negro se distribuyen como `.txt`, y sus definiciones apuntan al nombre correcto.
- Conserva los 21 luchadores, los 12 escenarios y todas las mejoras de 1.1.4. Se instala desde el mismo **COMBATE.exe**, sin reemplazar el lanzador.

### Contenido de 1.1.4 que se conserva

- Cuatro luchadores nuevos: **Ector “El Vaki”**, **Héctor “El Father”**, **El Conejo** y **El Negro**. El plantel sube a **21 personajes**, con los 12 escenarios anteriores.
- Selección ampliada a cuatro filas; se conserva **Al azar**. Los cuatro tienen retratos en la torre y pueden aparecer entre sus diez rivales.
- Ector usa sumo; Héctor conserva su Hirudora; El Conejo pelea con boxeo y contraataque.
- El Negro incluye sonidos de golpes y bloqueo, celebración de pie, reacciones al derribo de Rubén y una onda de rocas que avanza por el suelo. C mantiene llamas animadas durante el recorrido y en la estela.
- D consume una barra y C tres. Se conservan los modos, los niveles de dificultad y las asignaciones de controles de la versión anterior.

### Mejoras de 1.1.3 que se conservan

- Combos de ataques normales: **A → S → Z → X**, pulsando cada botón al conectar el golpe anterior. También hay cadenas cortas A → S → X y A → Z → X. El margen de entrada se amplía a seis cuadros, se reduce el retroceso de los golpes intermedios y cada impacto sucesivo reduce su daño. No hay cancelación en bucle.
- Levi, Isamar y Norwin conservan su movimiento evasivo con X: pueden hacer **A → S → Z** y salir con X.
- Los enlaces requieren acertar: un golpe fallado o bloqueado no habilita la cancelación al siguiente ataque.
- **Un control de consola + teclado:** en Jugador vs Jugador y 2vs2 Relevos, si se detecta exactamente un mando, **P1 usa el control** y **P2 usa flechas + A/S/Z/X/D/C**. La selección muestra la asignación. Conectá el control antes de elegir modo. Al volver al menú se restauran las asignaciones personales; la configuración guardada no se sobrescribe.
- Se conservan las dificultades Fácil, Medio y Difícil, el movimiento de CPU corregido, los 21 luchadores, los 12 escenarios, la selección Al azar y la torre de diez rivales.
- D requiere y consume una barra (1000); C requiere y consume tres barras (3000).

## Cómo actualizar

Cerrá el juego, abrí **COMBATE.exe → Buscar actualizaciones**, instalá **1.1.6** y elegí **Jugar**. Necesitás la instalación completa y el canal de actualizaciones configurado. Se puede actualizar directamente desde versiones anteriores.

El lanzador comprueba la firma del manifiesto y los hashes de los archivos, respalda el contenido sustituido y conserva save/config.ini, incluyendo controles y audio.

## Controles

| Situación | P1 | P2 |
| --- | --- | --- |
| Un mando en modo versus/relevos | Control de consola, con tus botones configurados | Flechas; A/S/Z/X ataques; D especial; C súper; Enter provocación |
| Sin mandos | Teclado configurado: de fábrica flechas + A/S/Z/X/D/C | Teclado configurado: de fábrica I/J/K/L + R/T/F/G/Y/H |
| Dos mandos | Primer control configurado | Segundo control configurado |

Para cubrirse, mantené la dirección contraria al rival. Escape abre la pausa. Q/W permiten las acciones de relevo cuando corresponda en el modo mixto. Podés personalizar los controles habituales desde Configuración. El archivo data/combate/COMBOS.txt incluye las indicaciones de esta versión.

## Validación

1.1.6: se verificaron firma, rutas, tamaños y SHA256 de los 108 archivos; se conservaron las 97 rutas previas (94 archivos idénticos y tres archivos de integración actualizados). Pasaron las pruebas del núcleo del actualizador: instalación, actualización, repetición, recuperación tras interrupción y conservación de controles/audio. Se decodificaron los sprites de ambos escenarios y El Poli, y se verificaron los 22 luchadores, 14 escenarios y todos los retratos anteriores de la torre. Las pruebas de combate recuperadas de El Poli registran daño, bloqueo, energía, proyectiles y derribo; no se repitieron en el motor en esta reconstrucción. La Turbina se reconstruyó desde la imagen adjunta y requiere una prueba visual en el juego Windows.

1.1.5: se reprodujo el fallo de 1.1.4 con el código del actualizador. La versión corregida se valida con el mismo decodificador de firmas y rutas, instalación completa, actualización desde una instalación previa, repetición de la actualización y conservación de controles/audio. Se verifican tamaño y SHA256 de los 97 archivos. Estas pruebas ejecutan el núcleo del actualizador en Linux; la interfaz de Windows no se ejecutó aquí.


1.1.4: los cuatro personajes se probaron en IKEMEN GO para Linux. Se comprobaron registro y retratos de selección/torre, energía y daño de los especiales de El Negro, recuperación tras el derribo y celebración de pie. El manifiesto firmado conserva las actualizaciones anteriores y no incluye configuraciones de usuario.


Pruebas del motor en Linux: combos de los 17 personajes con daño total esperado, cuatro golpes confirmados de El Sielvo (220), corte al fallar o bloquear, separación real del teclado de P1/P2 y retorno al menú. Se simularon cero, uno y dos mandos, incluyendo un mando con índice distinto de cero. Se verificó que las asignaciones guardadas no cambian.

Los mandos físicos y la interfaz Windows no se ejecutaron en ese entorno.

## Plataformas

Disponible para PC Windows. Android e iOS están en evaluación, sin versiones móviles publicadas ni fecha de lanzamiento.

Este repositorio distribuye actualizaciones de contenido; no contiene claves privadas ni una copia completa del motor.
