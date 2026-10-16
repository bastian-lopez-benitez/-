# Validación de Spectrite 1.14.0-almas-convergencia

La entrega es para Minecraft 1.21.1, NeoForge 21.1.172 y Java 21. El port a Forge 1.20.1 sigue documentado como trabajo posterior; el paquete de fuentes y recursos de bloques permite conservar sus IDs, modelos y recetas.

## Servidor y comportamiento

La batería completa ejecuta **196 pruebas en 34 suites**, con **0 fallos, 0 errores y 0 omitidas**, mediante servidores efímeros reales de NeoForge. Registros, efectos, recetas, botín, colisiones y eventos son los del motor. La ejecución final está en `build/convergence-final-build.log`; los XML originales permanecen en `build/test-results/test`.

Se comprueban los siguientes comportamientos:

- Vuelo de ambas transformaciones: permisos previos, salida, salud proporcional, guardado, reconexión, cambio de modo, dimensión y limpieza de concesiones huérfanas. No se devuelve salud gratis.
- Impactos repetidos de calaveras, flechas y cargas de fuego con daño periódico intercalado. Se conserva la inmunidad normal de las flechas vanilla. Los tres proyectiles del arco se tramitan individualmente, con guía, persistencia de munición y explosión sin daño de terreno.
- Forja: las 22 mejoras de las once piezas, costes, consumo y conservación de componentes; yunque con identidad propia, encantamientos y ojo activo. Orbes de Enderman al 5 % sin duplicar la tirada.
- Regeneración con hambre, inmunidad de quemadura nativa, fuerza limitada, almas por muertes, furia por impactos, tres saltos y fase del Wither a poca vida. Las nuevas habilidades mágicas de criaturas respetan esa fase.
- Monstruosidad: anuncios, ataques, salto físico, inmunidad a reflejo, efectos positivos de Spectrita II, botín y arena real guardada sin duplicar el jefe.
- Registro de las **39 especies hostiles vanilla**, 23 variantes añadidas, clases y atributos correctos. Vida y mejoras conservadas sin duplicarse ni curar al cargar.
- Registro de **25 mazmorras terrestres y cinco monumentos oceánicos**, sus dimensiones, estructuras, tablas de botín y poblaciones. Tres colocaciones escasas independientes, no una tirada por cada estructura.
- **300 planes terrestres** con rutas conectadas entre salas y plantas; 25 grafos distintos a igual semilla; trampas suficientes en las diez nuevas expediciones. Cinco huellas oceánicas distintas y conectadas: 5, 18, 21, 50 y 63 salas. Generación real de una cámara sumergida con aire encerrado y un campeón que no se duplica al guardar/reconstruir.
- Equipo por dificultad, presupuesto de 30 criaturas por spawner guardado y botín que aumenta con peligro; muertes atribuidas, límites contra granjas y materiales permitidos en encuentros finitos. Corazón y moldes monstruosos permanecen exclusivos de la Monstruosidad.
- Nueve familias de ataques: señales en posiciones fijas, posibilidad de esquivar, enfriamientos, obstáculos, daño real e inmunidad de quemadura. Esbirros de campeones con duración finita, sin objetos ni experiencia.
- Breeze: sustitución de su proyectil conservando dueño y movimiento; impactos sucesivos con los dos estados, ausencia de estados tras daño cero, daño saliente reducido exactamente un 25 %, velocidad reducida un 20 %, vaca que ataca y restaura su objetivo, ruptura temporal de facción y restauración al terminar Provocación.
- Carga cromática: empuje real exactamente doble que el de la carga vanilla, vidrio conservado, sin maldición al impulsarse uno mismo. Una Barra Spectral produce cuatro cargas. Perlas de Spectrita apilables a 32; perlas vanilla a 16.

## Cliente gráfico

El cliente real de Minecraft/NeoForge se abre con Xvfb y Mesa, dibuja **14 páginas de prueba** y se cierra normalmente con código 0. **50 comprobaciones aprobadas**, registradas en `build/client-probe/process-result.json` y archivadas en `previews/convergence/native-validation`.

Se comprueban y capturan armadura 3D de 425 cubos con diez placas interiores, escudo y guadaña en ambas manos, armadura de Almas Espectrales de 331 cubos en el inventario, once poses del jefe de 345 cubos, doce texturas de emisión, ocho fotogramas de la forja, barras compactas y temporizador, iconos de estado, seis modelos de bloques y materiales del Breeze. Los 23 nuevos proveedores de render y los dos del viento cromático se registran. El Códice real construye 48 páginas; los 30 nombres de encuentros y campeones tienen traducción y nombres únicos.

Las capturas son vistas técnicas de modelos e interfaces, sin crear un mundo. La colocación de piezas y el combate se verifican por separado en servidor. No se presenta esto como una partida multijugador manual ni como una prueba con todos los mods de terceros.

## Integridad y conservación

`tools/verify_jar.py` comprueba cada clase compilada, fuente integrada y recurso del proyecto frente al JAR final; detecta entradas ZIP duplicadas, corrupción, metadatos antiguos o pruebas incluidas en producción. Conserva todas las clases de la base 1.9.0-pre1 y las de la base histórica salvo el puente retirado de Soul Fire’d; la integración de fuego ahora pertenece al propio mod.

`tools/validate_resources.py`, `tools/validate_armor_rig.py` y `tools/validate_reaper_models.py` verifican JSON, recetas, referencias, traducciones, PNG, fotogramas, geometría y orientación. El JAR requiere Minecraft y NeoForge; Soul Fire’d, Prometheus y Cobweb ya no son obligatorios.

El ZIP de instalación contiene únicamente el JAR, con CRC y SHA256 comprobados. Los enlaces públicos se descargan completos y se comparan contra los archivos de entrega; el manifiesto y el resultado se conservan en `build/public-download-manifest.json` y `build/public-download-verification.json`.
