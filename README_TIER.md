# Spectrite: Señor de la Muerte

Fusión del JAR original y el archivo enviado `spectrite-1.21.1-1.9.0-pre1-almas.jar`, conservando sus sistemas y las mejoras posteriores. Versión **1.14.0-almas-convergencia**, para **Minecraft 1.21.1 / NeoForge 21.1.172 o posterior dentro de 1.21.1 / Java 21**. Instala la misma versión en cliente y servidor.

## Instalación

Coloca `spectrite-1.21.1-1.14.0-almas-convergencia.jar` en `mods`, sustituyendo el JAR anterior de Spectrite. Ambas versiones comparten el identificador `spectrite`; utiliza una sola.

El mod integra el sistema de fuego del JAR 1.9.0-pre1 y requiere Minecraft y NeoForge. Soul Fire’d, Prometheus y Cobweb ya no son dependencias obligatorias. El equipo existente conserva sus datos; los ascensos avanzados utilizan la Forja del Réquiem.

## Progresión y materiales

### Alma del Wither

En una mesa de crafteo:

```text
Calavera Wither    Calavera Wither    Calavera Wither
vacío             Estrella Nether    vacío
Arena de almas    Arena de almas     Arena de almas
```

Produce **1 Alma del Wither**. Las calaveras son las de esqueleto del Wither de Minecraft.

### Alma sobrecargada del Wither

El mismo patrón, usando **calaveras de esqueleto del Wither de Spectrita**, **estrella de Spectrita** y **arena de almas de Spectrita**. Produce **1 Alma sobrecargada del Wither**.

### Esencia de los No Muertos

En una mesa de herrería normal: deja vacía la ranura de plantilla y coloca un alma normal y una sobrecargada en los otros dos espacios. Acepta ambos órdenes y consume una unidad de cada alma. La esencia animada enlaza dos Withers como yin-yang, uno blanco prismático y otro negro de tonos oscuros.

### Rosa del Wither de Spectrita Oscura

Una rosa del Wither en el centro de la mesa de crafteo, rodeada de **8 fragmentos de gema de Spectrita**, produce una rosa oscura animada.

### Lingote de la Muerte

```text
Rosa oscura        Lingote almas activas    Rosa oscura
Lingote de almas   Esencia No Muertos       Lingote de almas
Rosa oscura        Lingote almas activas    Rosa oscura
```

Produce **1 Lingote de la Muerte**. Su animación recorre **hexágono → cuadrado → círculo → rombo → lingote**. Se conserva como material del tier y para repararlo. El ascenso a Señor de la Muerte utiliza ahora la esencia y el molde monstruoso en la nueva forja.

### Forja del Réquiem

Se fabrica en la mesa de crafteo con este patrón:

```text
vacío                         Yunque de Spectrita    vacío
Pala de Netherita Spectrita   Mesa de herrería       Hacha de Netherita Spectrita
vacío                         vacío                  vacío
```

Tiene un diseño de netherita con núcleo de Spectrita y yunque suspendido. Sus tres entradas son **molde → equipo base → material de ascensión**, más una ranura de resultado.

| Ascenso | Molde | Equipo base | Material | Experiencia |
| --- | --- | --- | --- | --- |
| Netherita Spectrita → Almas Espectrales | Molde de mejora de Almas Espectrales | Pieza correspondiente de Netherita Spectrita | 1 Lingote de almas activas | 20 niveles |
| Almas Espectrales → Señor de la Muerte | **Molde de mejora monstruosa** | Pieza correspondiente de Almas Espectrales | **1 Esencia de los No Muertos** | **30 niveles** |

Cada ascenso consume una unidad de las tres entradas. Las dos rutas incluyen **las once piezas**: casco, pechera, pantalones, botas, espada, pico, hacha, pala, azada, arco y escudo. Cada pieza Señor de la Muerte requiere su propio molde, incluidas armas y herramientas. Una victoria contra la Monstruosidad entrega cuatro moldes: suficientes para la armadura completa; las once piezas requieren once moldes.

La forja conserva nombre, encantamientos y datos del objeto, incluida la espada de sangre y las infusiones, y ajusta el desgaste proporcionalmente a la nueva durabilidad. Estos ascensos requieren el bloque real de Forja del Réquiem; el servidor comprueba proximidad, permisos, entradas y experiencia al fabricar y retirar el resultado.

### Yunque de Spectrita: encantamientos, reparación e infusión

El yunque de Spectrita conserva sus funciones de encantamiento y reparación. Para encantar, coloca el equipo a la izquierda y **un libro encantado** a la derecha. Respeta compatibilidad, límites de nivel y penalización de trabajos anteriores. En supervivencia, las operaciones de **40 niveles o más** quedan bloqueadas como «Demasiado caro». Consume un libro por operación.

El equipo Señor de la Muerte recibe nuevos encantamientos mediante este yunque real; la mesa de encantamientos, el yunque normal y la transferencia entre dos piezas no permiten eludir esa condición. No necesitas un molde para encantar o reparar. Repara Señor de la Muerte con Lingotes de la Muerte. El servidor valida que el bloque siga presente, tengas permiso y permanezcas a cuatro bloques o menos.

## Ojo Espía y orbes de Spectrita

Los Enderman normales y los Enderman de Spectrita tienen **un 5 % de probabilidad total de soltar un orbe de Spectrita** al morir con atribución a un jugador. Es una tirada fija: Saqueo no la aumenta y los dos tipos de Enderman no reciben tiradas duplicadas. La regla `doMobLoot` sigue aplicándose.

Combina **1 perla de ender de Spectrita + 1 polvo de blaze de Spectrita** para crear un **Ojo Espía de Spectrita**. Su silueta de ojo, iris y detalles prismáticos lo distinguen del orbe. El ojo reúne los siete poderes de los orbes y Fuerza de Spectrita II durante **15 segundos**: Furia, Ligereza, Prosperidad, Agilidad, Anfibio, Aguante y Resiliencia, todos a nivel II.

Puedes activarlo con **clic derecho** mientras lo sostienes, o infundirlo en una pieza de armadura del mod: **armadura a la izquierda + ojo a la derecha del yunque de Spectrita**, por **12 niveles**. La infusión consume el ojo y conserva el resto de datos. Lleva puesta una pieza infundida y pulsa **I** para activar los mismos poderes. También admite I con un ojo en cualquiera de las manos.

El ojo y todas las piezas infundidas comparten un único enfriamiento de **90 segundos por jugador**, persistente al morir o reconectar. Equipar más piezas o alternar ojos no multiplica el beneficio ni evita la recarga. La infusión añade una habilidad activa y conserva las infusiones pasivas de orbes que ya tuviera la armadura.

## Diseño y atributos

La etiqueta del tier es **☠ SEÑOR DE LA MUERTE · TIER SUPREMO ☠**. Los materiales tienen sprites propios de 128 × 128 y animaciones con transparencia. La armadura utiliza **425 cubos 3D**, atlas de 1024 × 1024 y 36 fotogramas, con emisión selectiva. La revisión cierra las zonas expuestas del cuerpo mediante placas y piezas interiores, conservando corona, cuernos curvos, máscara Wither, calaveras, costillas, núcleo de dos almas, manto, espina, faldones y garras.

Las herramientas conservan sus formas propias: mandoble, pico de garras, hacha de ejecución, pala funeraria, Guadaña del Ocaso, arco de costillas y escudo de tres almas. El escudo tiene **215 cubos**, volumen y orientación de bloqueo en ambas manos. La guadaña utiliza **146 cubos** con el filo hacia delante. El inventario de Almas Espectrales muestra su armadura mediante su modelo 3D nativo de **331 cubos**, con iluminación y profundidad.

| Propiedad | Señor de la Muerte |
| --- | --- |
| Durabilidad de herramientas | 18 000 |
| Velocidad de minado del material | 24 |
| Encantabilidad | 40 |
| Daño total espada / hacha / pico / pala / azada | 19 / 21 / 17 / 17,5 / 12 |
| Defensa casco / pechera / pantalones / botas | 9 / 18 / 14 / 9 |
| Dureza de armadura | 10 |
| Resistencia al retroceso por pieza | 0,35 |
| Multiplicador de durabilidad de armadura | 225 |
| Durabilidad arco / escudo | 5 760 / 5 670 |

El daño indicado incluye el punto base del jugador y excluye encantamientos y efectos. Sostener un arma, herramienta, arco o escudo Señor de la Muerte en la mano principal concede **Fuerza II**; no se añade una cadena de efectos ofensivos permanentes a cada herramienta. Las fórmulas y límites de defensa de Minecraft siguen aplicándose.

### Alcance de cuerpo a cuerpo por tier

El bono depende del equipo de la mano principal y desaparece al cambiarlo. Modifica el alcance de interacción con entidades, no la distancia de minado ni el alcance propio de proyectiles y habilidades.

| Tier | Bono sobre los 3 bloques habituales del jugador |
| --- | --- |
| Piedra | +0,10 |
| Hierro | +0,15 |
| Diamante | +0,20 |
| Netherita | +0,25 |
| Spectrita | +0,35 |
| Spectrita perfecta | +0,50 |
| Netherita Spectrita | +0,60 |
| Almas Espectrales | +0,80 |
| Señor de la Muerte | +1,00 |

## Pasivas del conjunto Señor de la Muerte

Los poderes de conjunto requieren las cuatro piezas correctas. El equipo conserva las habilidades compatibles de Almas Espectrales, evitando acumular dobles saltos o impulsos heredados.

**Regeneración de Spectrita II:** recupera **1 PV cada 25 ticks —1,25 segundos—**, como Regeneración II. Cada punto realmente recuperado genera **8 de agotamiento**: consume primero saturación y después hambre. Se pausa si el hambre llega a cero y no consume por intentos de curación a salud completa. Funciona pese al bloqueo de regeneración habitual. Matar un mob con atribución válida y equipo del tier o el conjunto completo restaura el hambre a **20**, la saturación a **6** y limpia el agotamiento; matar jugadores no repone comida.

**Cuerpo ignífugo de Spectrita:** evita la quemadura de almas/Spectrita identificada por el sistema del mod. El impacto físico de una calavera o flecha conserva su daño independiente. Tiene un icono propio de coraza y fuego protegido.

**Dos resurrecciones:** cada una devuelve 6 PV, Regeneración de Spectrita III durante 8 segundos y absorción temporal. Recuperas una carga cada **10 minutos de tiempo de servidor**, de forma sucesiva. El contador persiste al morir o reconectar; alternar con el tier anterior utiliza el mismo contador. No evita vacío, `/kill` ni fuentes técnicas de muerte. La regeneración posterior sigue consumiendo hambre.

**Coraza del Wither:** con el **25 % de salud o menos**, solo pueden dañarte ataques directos de cuerpo a cuerpo; se muestra la energía deslizante del Wither sobre el modelo de la armadura. También se aplica a la reserva de ambas transformaciones. Los proyectiles enemigos se desvían manteniendo velocidad, dueño y dirección general de avance. Perlas y anzuelos conservan su uso. Vacío, `/kill` y fuentes técnicas de muerte mantienen su comportamiento.

**Tres saltos aéreos e inmunidad a caídas:** el salto normal y tres pulsaciones adicionales de Espacio suman cuatro saltos por trayecto. Se recuperan al tocar el suelo y no se activan al nadar, trepar, montar, planear o volar como Wither. Cada salto reproduce el lanzamiento del Wither y deja caer una poción persistente real: nube de dos bloques de radio, cinco segundos de vida y Wither I de cinco segundos. Respeta dueño, aliados, mascotas y PvP.

| Pieza | Pasiva individual |
| --- | --- |
| Casco | Mirada del Sepulcro: señales sobre hasta seis enemigos visibles a 8 bloques, sin revelar a través de paredes. |
| Pechera | Última Guardia: al recibir daño y quedar al 30 % de vida o menos, Absorción I durante 3 s; recarga de 45 s. |
| Pantalones | Paso del Sepulcro: +0,15 al atributo de velocidad al agacharse en el suelo. |
| Botas | Con equipo parcial, −50 % de daño de caída durante los 3 s posteriores al dash. Con el conjunto completo, inmunidad a caída. |

## Almas, furia y controles

Las teclas se pueden reasignar en Opciones → Controles. La barra de almas tiene un máximo de **100** y se llena **solo mediante muertes confirmadas**: **20 almas con la Guadaña del Ocaso**, **10 con las demás armas/herramientas del tier o usando el conjunto completo**, y **5 por baja durante cualquiera de las transformaciones**. Lanzar calaveras al aire, golpear sin matar, bloquear o causar daño periódico sin baja no genera almas.

Los proyectiles conservan el arma de origen; cambiarla después no mejora la recompensa. El daño periódico conserva una ventana de atribución de cinco segundos desde el último golpe válido. Una resurrección no cuenta como muerte y cada baja se paga una sola vez.

La **furia vuelve a coexistir con las almas**: cada impacto válido concede cuatro puntos, como Netherita Spectrita, con un intervalo mínimo de diez ticks; hacen falta 25 impactos para completar 100 puntos. Pulsa **U** para activar **20 segundos** de **+15 % de velocidad de ataque y +10 % de movimiento**. Este tier no recibe además el multiplicador de daño de furia de tiers anteriores. Durante ambas formas Wither no se carga ni se activa furia y ambas barras se sustituyen por un reloj de transformación.

| Control | Habilidad | Coste y límites |
| --- | --- | --- |
| V | Equilibrio eterno: alterna alma blanca defensiva y negra ofensiva | Blanca: −15 % de daño recibido. Negra: +15 % de daño directo de cuerpo a cuerpo y calaveras. Cambio cada 2 s; no se acumulan. |
| G | Mandato del Sepulcro: hasta dos guardias | 40 almas; duración 15 s; recarga 45 s. Cada guardia tiene 20 PV y causa 4 de daño base, como máximo una vez por segundo. |
| H, mirando a un aliado | Custodia funeraria: asigna un guardia existente | 20 almas; hasta 8 s; recarga 30 s. No crea guardias ni alarga su vida original. |
| B, mirando a un enemigo | Sello del Sepulcro | 20 almas; bloqueo de teletransporte durante 3 s; recarga 30 s. Jefes inmunes. Solo una perla de ender de Spectrita real puede atravesarlo. |
| Tres golpes primarios cargados al mismo enemigo | Juicio de las Tres Cabezas | Hasta 5 s entre golpes; el tercero suma 8 de daño base y Wither I de 3 s; recarga 10 s. Bloqueos y barridos no cuentan. |
| Clic derecho con el conjunto completo | Calavera central | 8 de daño base, Wither II de 3 s y quemadura de almas de 4 s; una por segundo. Admite guadaña o mano vacía, respetando arco, escudo, comida y bloques. |
| Agacharse + mantener clic derecho 3 s con mandoble o hacha | Calavera de Spectrita cargada | 10 almas; 14 de daño base; recarga 3 s. Soltar antes cancela la carga. |
| Agacharse 5 s en el suelo con la guadaña principal | Wither normal | Conjunto completo; 300 PV, 20 s, sin coste de almas; recarga compartida de 180 s. |
| R con 100 almas y la guadaña principal | Wither de Spectrita | Conjunto completo; consume 100 almas; 750 PV, 25 s; recarga compartida de 180 s. R también termina antes la forma actual. |

Custodia y Sello seleccionan el primer objetivo bajo la mira hasta 16 bloques, con visión directa. Una selección inválida no gasta recursos. Custodia admite aliados y sus mascotas, mantiene al protegido a 24 bloques o menos y devuelve el guardia al dueño al terminar. El Sello bloquea perlas normales, chorus, Enderman, portales y teletransportes durante su duración; no bloquea caminar. La excepción exige el impacto de la perla de Spectrita y su dueño: llevar una en el inventario no permite otro teletransporte. Los enfriamientos persisten y se respetan protecciones externas.

### Guadaña del Ocaso: maldiciones y cosecha

Cada golpe directo que cause daño aplica **Wither I**, **Robo de alma** y **Aberración cromática descompuesta** durante cinco segundos.

- **Robo de alma:** el daño real recibido por la víctima cura al propietario original de la marca un **25 %**. Está limitado a **2 PV por segundo en total para el portador**, aunque marque una multitud, y a **6 PV por marca**. Respeta el bloqueo normal de curación, aliados y mascotas. Cambiar de arma no roba la propiedad de una marca ajena.
- **Aberración cromática descompuesta:** reduce un **25 % la defensa de armadura efectiva**, causa **2 de daño periódico por segundo**, el doble de la aberración normal, y bloquea la regeneración/curación habitual. Sustituye la aberración normal para evitar dos versiones acumuladas. Los jefes con Bloqueo de negación de regeneración conservan su curación.
- **Tres marcas de cosecha:** tres golpes primarios cargados al mismo enemigo, con hasta 5 s entre ellos, añaden 4 de daño base y Wither II durante 4 s al tercero. Recarga por víctima de 8 s. No cuentan barridos, fallos ni golpes bloqueados.

### Arco del Trono del Vacío

Cada disparo válido libera **tres calaveras guiadas de Wither de Spectrita**, con salida en abanico −6°, 0°, +6°. Fijan un enemigo visible en un cono de 24 bloques al disparar; su giro es limitado y pierden la guía si el objetivo deja de ser válido. La guía se valida de nuevo contra aliados, equipos, PvP y paredes. El disparo consume una munición y un punto de durabilidad, respetando Infinidad y creativo. Cada calavera causa **16 × fuerza de carga** de daño base, antes de encantamientos y defensas.

Los impactos provocan un estallido de combate de 1,75 bloques: daño secundario limitado al 25 % del directo, sin duplicar daño a la víctima principal, sin destruir bloques ni invocar explosiones del terreno. Aplican Aberración cromática y quemadura de Spectrita durante 4 s (5 con Llama). La munición decide el Wither: normal II durante 5 s; flecha de Spectrita III más daño persistente durante 6 s; flecha perfecta IV más daño persistente durante 8 s. La carga completa también puede aplicar Corrupción. El daño persistente provoca 2 PV/s y la Resistencia fracturada hace que las armas de Spectrita ignoren el 20 % de la armadura mientras dure; el icono muestra un escudo roto. Esta marca se renueva sin acumular porcentajes ni modificar permanentemente los atributos.

Las dos flechas de Spectrita se fabrican con **varilla de diamante**, punta correspondiente y pluma, produciendo cuatro. Dos diamantes en vertical producen **seis varillas de diamante**. El impacto básico de Spectrita conserva su penetración del 15 % antes de la marca; el 20 % de la marca sustituye ese porcentaje.

### Arco de Almas Espectrales

Ahora libera **un pulso sónico por disparo**, en lugar de la doble flecha anterior. Su fuerza sigue la curva de carga del arco: **daño base = 4 + 12 × carga** y **alcance = 8 + 32 × carga**, hasta **16 de daño base y 40 bloques** al máximo. Las paredes recortan su recorrido. Consume una munición por descarga y conserva los encantamientos compatibles y sus reglas de consumo. Es una alternativa de tiro lineal que no persigue enemigos.

### Escudo: repulsión y tres calaveras guiadas

Con el escudo levantado, usa **agacharse + clic derecho**, el gesto de ataque mientras bloqueas, o **X mientras bloqueas** para activar la repulsión sónica. Tiene **8 s de enfriamiento**, inflige **6 de daño base** y empuja a los enemigos de la zona frontal.

El escudo Señor de la Muerte añade **tres calaveras guiadas** contra el enemigo visible bajo la mira. Cada una causa **6 de daño base**, no explota y añade **3 segundos de Wither** al que ya posea la víctima, con un máximo de **10 segundos** y sin rebajar su nivel. Si no hay objetivo válido conserva la repulsión, sin crear calaveras que busquen objetivos arbitrarios. La descarga del escudo utiliza su propia guía y sus propias reglas de daño y Wither. La Monstruosidad es inmune al daño reflejado por parada o espinas.

### Arsenal: Z, X y C

**Z, Paso funerario:** avanza hasta siete bloques en medio segundo, con colisión real. Cada enemigo alcanzado recibe una sola vez 6 de daño base y Wither I de 3 s. Recarga de **10 s**. Con el conjunto completo cuesta **15 almas**; sin él, una herramienta o escudo del tier y **8 de durabilidad**. Montar, planear o usar un objeto impide activarlo. La forma Wither dispone de su propia carga.

**X:** con las cuatro piezas cuesta 10 almas, salvo la guadaña, que cuesta 15; sin el conjunto consume 8 de durabilidad del objeto. Las habilidades de la tabla comparten recarga, por lo que cambiar de herramienta no permite encadenarlas.

| Equipo | Habilidad de X | Efecto y recarga |
| --- | --- | --- |
| Mandoble | Corte del Umbral | Tajo frontal de 5 bloques; 8 de daño y Wither II de 4 s; 12 s. |
| Hacha | Ejecución del Sepulcro | Frontal de 3,5 bloques; 8 de daño y Lentitud II de 3 s; 14 s. |
| Pico | Fractura espectral | Frontal de 6 bloques; 6 de daño, Debilidad I de 4 s y Prisa I propia de 6 s; 16 s. |
| Pala | Fosa de almas | Frontal de 5 bloques; 4 de daño, Lentitud III de 3 s y disipación de proyectiles enemigos visibles; 16 s. |
| Guadaña | Cosecha del Segador | Barrido de 150° y 5 bloques; 10 de daño y Wither II de 4 s; si logra bajas cura hasta 2 PV por activación; 10 s. |
| Guadaña + agacharse | Cadenas del Parca | Objetivo visible a 12 bloques; atrae hasta 3 bloques con colisión y aplica Debilidad I de 3 s; jefes inmunes; 18 s. |
| Arco | Salva de ánimas | Prepara durante 8 s el siguiente disparo completamente cargado: solo la calavera central añade Lentitud II de 3 s; 18 s. |
| Escudo, sin bloquear | Bastión funerario | Durante 4 s reduce un 30 % el daño frontal admisible y contraataca una vez a cada atacante visible cercano, hasta cuatro, con 4 de daño y Wither I de 3 s; 20 s. |

La selección de X prioriza la mano principal; para usar el escudo secundario, sostén delante un objeto sin habilidad del arsenal. Los ataques comprueban aliados, mascotas, PvP y visión. Los efectos ofensivos requieren daño real. Z y C tienen recargas independientes de X.

**C, Corrupción voluntaria:** conjunto completo, 20 almas, duración de **12 s** y recarga de **40 s**. Reduce tu vida máxima un 25 %. Tus golpes primarios cargados que causen daño generan un tajo frontal de 6 bloques, con 4 de daño y Wither II de 3 s, como máximo cada 16 ticks. Las paredes detienen el tajo y no se repite con barridos o daño secundario. Recuperar el máximo al terminar no devuelve salud. Quitar equipo, transformarte, morir o cambiar de dimensión cancela la postura; no elimina la maldición enemiga de Corrupción.

## Dos formas Wither

Ambas requieren mantener **las cuatro piezas y la Guadaña del Ocaso en la mano principal**. El Wither normal se prepara agachándose cinco segundos en el suelo, dura 20 s y concede una reserva de 300 PV; el de Spectrita consume 100 almas con R, dura 25 s y concede 750 PV. Comparten 180 s de enfriamiento desde la activación.

Mantienes inventario y equipo. El render muestra el Wither de tres cabezas; la forma de Spectrita utiliza 36 fotogramas prismáticos. **WASD mueve, el ratón apunta, Espacio asciende y agacharse desciende**. Clic derecho dispara la cabeza central. Las laterales disparan cada dos segundos por cabeza a enemigos válidos y visibles hasta 20 bloques. Son inmunes a fuego, Wither y veneno y recuperan 1 PV por segundo con la regeneración propia de la forma, además de la pasiva del conjunto.

La colisión de la transformación rompe hasta 12 bloques por tick, con permisos y eventos normales, de dureza **menor que 50**. Obsidiana normal, obsidiana de Spectrita, bloques más duros e irrompibles permanecen protegidos. Las calaveras no destruyen terreno.

| Control transformado | Ataque | Límites |
| --- | --- | --- |
| X, Wither normal | Salva de las tres cabezas hacia un punto fijado al iniciar | Aviso de 1 s; alcance de selección 20 bloques; recarga 6 s. |
| X, Wither de Spectrita | Ciclo salva triple → onda de almas → lluvia de seis calaveras | Aviso de 1 s; recarga 6 s. Onda de 2 a 10 bloques, saltable, 6 de daño y Wither II de 5 s. La lluvia comprueba paredes y techos. |
| Z, ambas formas | Carga horizontal de hasta 7 bloques en medio segundo | Una vez por enemigo: 6 de daño y Wither I de 3 s; recarga 8 s. Respeta colisión, borde del mundo y zonas cargadas. |

X y Z no gastan almas ni durabilidad durante la forma y no se inician uno durante la ejecución del otro. La forma de Spectrita intenta invocar refuerzos al bajar al 30 % de reserva: una sola vez por transformación, hasta dos guardias de 15 s compartiendo el límite existente.

R termina antes la forma. También termina al perder una pieza, cambiar la guadaña, morir, salir, cambiar de dimensión o dejar de cumplir las condiciones. Se restaura el estado de vuelo previo; el permiso temporal se limpia igualmente al reconectar y en las rutas de interrupción. La velocidad de vuelo temporal no queda incorporada al jugador.

Al salir se restaura el máximo habitual de salud y se conserva, como máximo, el menor valor entre la salud de entrada y el máximo habitual multiplicado por la fracción de reserva restante. Entrar con 16/20 PV y salir con media reserva deja como máximo 10/20 PV: la transformación no concede curación gratuita. Durante la forma la interfaz oculta las barras de almas y furia y muestra el **tiempo restante de transformación**.

## Monstruosidad de Spectrita

Jefe inspirado en la Monstruosidad de Redstone de Minecraft Dungeons, reinterpretado como **gólem de netherita** con piezas de Spectrita. Sus zonas metálicas oscuras conservan reflejos y remaches; las partes prismáticas utilizan el patrón de Spectrita mediante **12 fotogramas de emisión**. Tiene **345 cubos 3D**, atlas de 1024 × 1024, cuernos, pinchos de asedio, garras, mandíbula, iris y pistones articulados. La barra propia combina un marco de netherita, facetas prismáticas animadas y porcentaje de salud en un formato compacto.

### Invocación

Craftea un Corazón de la Monstruosidad:

```text
Rosa oscura     Lingote almas activas     Rosa oscura
Lingote activo  Estrella de Spectrita     Lingote activo
Rosa oscura     Lingote almas activas     Rosa oscura
```

Úsalo en la cara superior de un suelo sólido de **5 × 5 bloques**, con **seis bloques de altura libre**. Se consume al invocar correctamente. Se comprueban espacio, permisos, dificultad y que no haya otra Monstruosidad a menos de 128 bloques. En creativo también existe `/summon spectrite:spectrite_monstrosity`.

### Combate

Tiene **1024 PV**, **18 de armadura** y **12 de dureza**. El núcleo cerrado reduce el daño entrante un 35 % antes de los efectos defensivos. Acumular presión lo expone durante cinco segundos y cada ataque deja una recuperación. Conserva los efectos positivos de Spectrita, Regeneración de Spectrita I y **Bloqueo de negación de regeneración**, además de beneficios de combate definidos; conserva su curación pese al bloqueo de la aberración. Aguante I y Resistencia I reducen el daño ordinario de forma sucesiva, sin convertirlo en invulnerable. Los ataques normales y proyectiles que superen sus defensas pueden dañarlo.

Rota **ocho ataques**, con avisos y recuperación finitos:

| Ataque | Respuesta del jugador |
| --- | --- |
| Martillos de asedio | Levanta ambos brazos antes del golpe; después emite una onda saltable. Aléjate del impacto y salta la onda. |
| Láser prismático | Sigue al objetivo durante el aviso, fija su dirección y dispara después; se puede esquivar y las paredes lo detienen. |
| Minas de cristal | Marca las posiciones antes de detonar; cada mina tiene fusible propio y el número activo está limitado. |
| Embestida | Prepara una carrera en línea, que usa colisión física. Apártate de su dirección y aprovecha la recuperación. |
| Rayos de Spectrita | Fija una zona de 2,4 bloques de radio y la golpea después con 8 de daño base. Sal de la marca; el rayo visual no crea fuego ni un segundo impacto. |
| Pociones persistentes | Lanza tres botellas reales con arco balístico, creando nubes de daño de Spectrita de radio 3 y duración de 6 s. Muévete y abandona las nubes. |
| Boom sónico | Fuente de daño del Warden: 10 de daño base en Normal, 6 en Fácil y 15 en Difícil; hasta 32 bloques. Fija la dirección antes de disparar y puede atravesar paredes: esquívalo lateralmente. |
| Supersalto | Aviso de 1,5 s, despegue con gravedad y aterrizaje real. El impacto causa 20 de daño base y su onda 12, una sola vez por víctima; solo golpea a jugadores en el suelo. Salta al caer el jefe. |

**Fractura del reactor** abre una ventana de contraataque. Al cruzar la mitad de salud inicia una sola vez la **Sobrecarga**, con tres ondas escalonadas y una segunda fase más rápida. Las nuevas animaciones se vinculan al reloj de ataque del servidor; el golpe del supersalto coincide con su aterrizaje real.

Cada ventana ofensiva registra una oportunidad de contacto por jugador: bajar el escudo después de bloquear no crea otro golpe del mismo rayo u onda. Respeta aliados y no selecciona jugadores creativos o espectadores. Es inmune a espinas y al daño de proyectiles marcados como reflejados; no vuelve inmune a todo proyectil normal.

Puede romper hasta **12 bloques de contacto por tick**, incluidos materiales duros rompibles, cuando `mobGriefing=true` y los eventos de protección lo permiten. No rompe bloques de dureza negativa, contenedores ni los cimientos por debajo de sus pies. Esta limitación conserva una pelea destructiva sin borrar una región completa de golpe.

### Recompensa

Una muerte atribuida a un jugador entrega **4 Moldes de mejora monstruosa + 8 Lingotes de almas activas + 16 Lingotes de almas + 8 bloques de Spectrita + 1 corazón de la Monstruosidad**. El molde no se fabrica ni se duplica. Cuatro moldes permiten ascender la armadura completa en la Forja del Réquiem con sus cuatro piezas de Almas Espectrales, cuatro esencias y 30 niveles por pieza. Las armas y herramientas requieren igualmente un molde por ascenso. `doMobLoot=false` desactiva el botín.

## Daño de Spectrita y presentación

**Daño instantáneo de Spectrita I** causa **15 de daño base**, 2,5 veces los 6 de Daño instantáneo I. Los niveles siguientes siguen su escala. Ignora las reducciones de armadura, resistencia y protección mágica correspondientes a este daño; mantiene la atribución del atacante, el control de aliados y las protecciones técnicas del servidor. Las nubes y exposiciones parciales conservan el escalado propio de las pociones persistentes. No borra globalmente las ventanas de invulnerabilidad de cualquier entidad.

Los efectos tienen iconos dedicados, incluidos Daño persistente y Resistencia fracturada. También se conservan los seis anteriores: Regeneración de Spectrita, Cuerpo ignífugo, Robo de alma, Aberración descompuesta, Bloqueo de negación de regeneración y Daño instantáneo de Spectrita.

La interfaz mantiene almas y furia en **barras más pequeñas**, separadas del hambre. **F8** alterna presentación **compacta → completa → oculta**. **F9** alterna partículas **reducidas → ocultas → todas**. Estas preferencias son del cliente y se guardan. Los avisos de combate del jefe conservan su propósito de anticipar ataques. Durante una transformación aparecen su reloj y su reserva de vida, sin superponer las dos barras humanas.

## Propuestas de habilidades adicionales — no implementadas

Estas son ideas opcionales para una actualización futura; no forman parte del JAR descrito.

| Tier | Propuesta | Balance propuesto |
| --- | --- | --- |
| Señor de la Muerte | Edicto del Último Latido: consumir una marca de Robo de alma para interrumpir brevemente a una criatura común | 25 almas; 0,75 s; recarga 35 s; jefes y jugadores inmunes. |
| Señor de la Muerte | Procesión de Ceniza: convertir la siguiente muerte cercana en un sello que ralentice a enemigos | 15 almas; radio 3; duración 4 s; recarga 25 s; sin daño ni acumulación de sellos. |
| Señor de la Muerte | Testamento del Trono: gastar la mitad de las almas guardadas para proteger a un aliado de un único golpe | Mínimo 40 almas; reducción máxima del 30 % durante 3 s; recarga 90 s; no concede otra resurrección. |
| Almas Espectrales | Eco de prospección: revelar durante unos segundos minerales ya expuestos cercanos | Radio 8; recarga 30 s; no revela a través de bloques sólidos. |
| Almas Espectrales | Resonancia del camino: un breve bono de minado después de atravesar un corredor estrecho | Prisa I de 4 s; recarga 20 s; no se acumula con otra Prisa superior. |
| Almas Espectrales | Ancla de cooperación: enviar una señal visible solo a aliados y darles orientación hacia ti | Duración 8 s; recarga 25 s; sin teletransporte, curación ni detección de enemigos. |

## Reconstrucción y validación

El JAR original permanece en `libs` como base de compilación y para fusionar el contenido sin cambios. `reference` contiene fuentes del JAR y queda fuera de la compilación; las modificaciones están en `src/main` y las pruebas en `src/test`. En el entorno Linux de desarrollo:

```bash
cd death-lord
python3 tools/setup_jdk.py
python3 tools/gradle.py test jar --console=plain
python3 tools/validate_resources.py
```

La validación PNG requiere Pillow. Gradle, NeoForge y dependencias tienen versiones fijadas; los descargadores mantienen verificación TLS e integridad. El JAR se copia a `dist`.

`tools/generate_resources.py` reproduce recetas, etiquetas y traducciones. Los scripts artísticos conservan las pinturas originales en `previews` y realizan su integración técnica en los atlas. El modelo Overlord conserva el contrato de `tools/armor_uv_contract.json`; el jefe utiliza `tools/monstrosity_uv_contract.json`. La forja y los efectos tienen sus propias fuentes de arte conservadas. Consulta **VALIDACION.md** para resultados de pruebas y comprobaciones gráficas reales, sus evidencias y sus límites.

Autoría original conservada: FlashfyreDev y los autores del port y de Almas Espectrales. Esta modificación parte del archivo adjunto para uso del solicitante y conserva las licencias del contenido previo y sus dependencias.

## Veinticinco mazmorras, criaturas y arquitectura

Quince expediciones del Overworld y diez del Nether, con dificultad I–V y mapas de cartógrafo que muestran destino real, dimensión y dificultad. Los diez nuevos recorridos son Laberinto de Obsidiana, Catedral Quebrada, Panóptico Abisal, Sepulcro del Relojero y Corona de la Ruina, más Prueba Infernal, Laberinto del Magma, Cadenas Sepulcrales, Ciudadela del Fuego Eterno y Eclipse del Nether. Los nuevos recorridos tienen al menos 75 salas y tres plantas; los de grado V suelen tener 120–160 salas y cuatro plantas. La Fundición Monstruosa mantiene 160–184 salas y su gran arena. Hay rutas laterales, ocho decoraciones de sala, refugios con suministros, trampas de proyectiles/pociones/fuego, fosos, suelo falso y cargas explosivas con señales visibles.

El Nether comparte una colocación extremadamente rara: celdas de 160 chunks, separación 80 y frecuencia 0,15 para el conjunto, sin multiplicar esa frecuencia por cada nueva estructura. Las entradas buscan suelo real bajo el techo de bedrock. Los cartógrafos maestros venden las expediciones más difíciles y del Nether; el Códice tiene 48 páginas.

**Las 39 especies de la categoría hostil de Minecraft 1.21.1 tienen contraparte de Spectrita**: se conservan las existentes y se añaden 23. El cubo de magma aparece en fortalezas de Spectrita y mazmorras del Nether. La población cambia por dimensión y dificultad, con guardianes de élite únicos en cámaras concretas; los jefes globales no aparecen en spawners comunes. Las nuevas variantes conservan anatomía/animaciones de su especie y una capa cristalina prismática. Reciben 60 % más vida y 25 % más daño que su especie base, con modificadores persistentes que no se duplican al cargar el mundo.

Los mobs de Spectrita coordinan como máximo tres aliados ociosos cercanos con visión del objetivo; los terrestres compatibles tienen flanqueo corto, retirada de atacantes a distancia y maniobras ante proyectiles, con pausa y comprobación de ruta. Su escolta invocada mantiene su IA propia. La coordinación no detecta jugadores a través de paredes y excluye creativo/espectador.

El equipo escala desde cota de mallas a Spectrita y Netherita Spectrita; nunca se obtiene gratuitamente el equipo avanzado que lleva un guardián. Los materiales adicionales, probabilidad, cantidades y experiencia aumentan según el peligro de la especie. El botín adicional exige una muerte atribuida a jugador. Los spawners de mazmorra tienen un presupuesto persistente de 30 criaturas: sus bajas pueden entregar materiales, respetando el límite regional contra granjas. Spawners ordinarios ilimitados conservan las restricciones. El corazón y los moldes monstruosos siguen reservados a la Monstruosidad.

Seis bloques nuevos usan las texturas animadas del JAR: mosaico, relieves, baldosas, pilar fracturado, cúmulo y relicario de fragmentos de Spectrita. Aparecen integrados en suelos, esquinas y salas, conservando libres puertas, escaleras y trampas. El mosaico se fabrica con pizarra profunda y cuatro fragmentos; el resto utiliza un mosaico y cuatro fragmentos.

## Port final a 1.20.1

Se conservan fuentes, generadores, modelos, recetas e identificadores de los bloques. `PORT_1_20_1.md` documenta los cambios de motor necesarios y `tools/export_1_20_1_fragment_assets.py` exporta los recursos de los seis bloques al formato 1.20.1. Esos recursos se integrarán en el port de Forge; **el JAR actual es para 1.21.1**. El paquete de recursos exportado no sustituye un mod compilado para 1.20.1.

## Monumentos oceánicos y encuentros finales

Además de las 25 mazmorras terrestres hay **cinco monumentos submarinos**: Arrecife del Prisma (II), Basílica Sumergida (III), Relicario Abisal (IV), Ciudadela de las Mareas (IV) y Santuario del Leviatán (V). Tienen, respectivamente, 5, 18, 21, 50 y 63 cámaras. Sus plantas son cruz de coral, naves en dos niveles, anillo con conexiones radiales, fortaleza vertical de cobre y santuario abisal de tres niveles. Incluyen cámaras inundadas, guardianes y ahogados de Spectrita, bloques de fragmentos, cofres, spawners limitados, trampas de burbujas descendentes y campanas de vidrio que conservan aire. Solo se colocan en biomas oceánicos y bajo el nivel del mar, con espacio real para todas sus plantas. Comparten una colocación escasa: 96 chunks, separación 48, frecuencia 0,25.

Cada expedición tiene un jefe final nombrado: **29 campeones y la Monstruosidad**. Los campeones utilizan la anatomía animada de su especie de Spectrita, vida ajustada al grado, barra de jefe, recompensas adicionales y combinaciones de ataques que cambian por perfil. Los cinco monumentos tienen arcontes Guardianes ancianos con un anillo de marea y un segundo ataque diferente. Los campeones se guardan en NBT y no se duplican al reconstruir piezas. Solo la Monstruosidad suelta su corazón y el Molde monstruoso.

Las 25 mazmorras terrestres tienen reglas propias de conexiones: anillos, ramales funerarios, minas con eje y galerías, canales, patios, diagonales, naves amplias, cámaras de prisión, archivos de pasillos alternos y recorridos de prueba en serpentina. Sus materiales, puntos de referencia, población, longitud y jefe se combinan por perfil; no son copias de una planta con otro color. Las salas incorporan talleres cristalinos, relicarios, observatorios, rieles, celdas, hornos, archivos, vitrales, braseros y refugios de suministros.

Los mobs de Spectrita incorporan nueve familias de habilidades: fractura cromática, descarga prismática, anillo de mareas, ceniza ardiente, salto de caza, égida, miasma, sombra y vendaval. Anuncian una posición y dejan 24 ticks para esquivar; los campeones avisan durante 30 ticks y alternan más patrones. Los impactos comprueban alcance, visión, aliados y daño efectivo. Los ataques mágicos respetan la fase del Wither a poca vida. Los campeones pueden convocar hasta dos esbirros temporales; desaparecen en 15 segundos y no dan objetos ni experiencia.

## Breeze y viento cromático

El **Breeze de Spectrita** tiene cuerpo y remolino prismáticos. Habita el Santuario, el Observatorio del Eclipse, el Sepulcro del Relojero y la Corona de la Ruina; también hay campeones de su especie en los encuentros adecuados. Sus proyectiles se convierten en entidades de viento de Spectrita reales, conservando dueño y trayectoria.

Un impacto que cause daño aplica **Provocación durante 8 s** y **Debilidad cromática durante 8 s**. Provocación atrae mobs hostiles, neutrales y pasivos cercanos en un radio de 16 bloques; pueden perseguir y atacar a la víctima, incluso los animales. Al terminar restaura sus objetivos anteriores. Respeta equipos, mascotas propias y escoltas del Señor de la Muerte. Los jefes mantienen su IA y resisten la marca de Provocación, que sobre ellos dura 2 s. Debilidad cromática reduce una sola vez el daño causado un 25 % y la velocidad un 20 %, sin acumular porcentajes.

Los Breezes derrotados con crédito de jugador sueltan **1–2 Barras Spectral**, además del botín de peligro correspondiente y de las restricciones de spawners. Su diseño es una vara de viento de marfil/plata con espirales, claramente distinta de la vara ígnea de Blaze de Spectrita. Una Barra Spectral se descraftea en **4 cargas de viento cromáticas**. Se pueden lanzar a mano o con dispensador: el mismo radio que la carga vanilla, multiplicador de empuje **2,44 frente a 1,22**, exactamente el doble; no destruyen bloques. El impacto directo en otra criatura aplica los dos estados. Impulsarte contra el suelo no te maldice a ti mismo. Tienen medio segundo de recarga.

Las **perlas de ender de Spectrita se apilan hasta 32**. La perla vanilla sigue en 16.
