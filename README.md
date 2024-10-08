Prácticas de aula 6 (PA06): Distribución de especies, patrones de
distribución por simple inspección<small><br>Biogeografía
(GEO-131)<br>Universidad Autónoma de Santo Domingo (UASD)<br>Semestre
2024-02</small>
================
El Tali
2024-10-08

Versión HTML (quizá más legible),
[aquí](https://biogeografia-master.github.io/patrones-distribucion-simple-inspeccion/README.html)

# **Fecha/hora de entrega**

**8 de octubre de 2024, 7:59 pm.**

# **Introducción**

En esta práctica, trabajaremos con la distribución espacial de especies
utilizando registros de presencia obtenidos de GBIF (Global Biodiversity
Information Facility). El objetivo es realizar una inspección visual de
los patrones de distribución y posibles asociaciones con factores
ambientales como elevación, pendiente, geomorfología, y tipos de
vegetación. No se requiere el uso de R o Python para cálculos complejos
(sólo opcionalmente), sino que te apoyarás con mapas provistos en clase
o enlaces a mapas.

Debes seleccionar un taxón (especie o género) con al menos 500 registros
de presencia en República Dominicana, de modo que puedas observar su
distribución a nivel nacional. A partir de esto, explorarás si existen
patrones espaciales claros o asociaciones con elementos del medio
físico. Tan pronto selecciones tu taxón, anúncialo en el foro.

Hay muchas guías para hacer búsquedas en la [API web de
GBIF](https://www.gbif.org/), y también hay muchas maneras de hacerlo.
Mi recomendación: entra en la API web, presiona sobre `Occurrences`,
luego en la caja `Search all fields` escribe el taxón, no presiones el
botón de lupa aún, ve abajo a `Country or area`, busca
`Dominican Republic` (no elijas `Dominica`), verifica el número de
registros, si supera los 500 registros, elígelo y trabaja con él. Puedes
luego visitar la opción de mapa, el cual seguramente te mostrará
registros fuera de RD (ignora estos últimos y concéntrate en RD).

------------------------------------------------------------------------

# **Ejercicio 1: Selección de taxón y análisis de registros de presencia**

1.  Elige un taxón (especie o género) con al menos 500 registros en GBIF
    para República Dominicana. Si no sabes alguno, pregunta al ChatGPT
    cuáles especies o géneros podrían estar bien representados.

2.  Explora su distribución visualmente usando los mapas provistos en el
    aula. Estos mapas incluirán información dle medio físico o
    “ambiental”, pero no tienes que limitarte a estos:

    - Mapa geológico. Existe
      [este](https://geofis.xyz/lm/index.php/view/map/?repository=geo250krd&project=geologico_gpkg)
      interactivo, pero seguramente no abrirá con rapidez. Puedes
      intentar con [este PDF del Servicio Geológico Nacional
      (SGN)](https://sgn.gob.do/images/docs/mapa_geologico.pdf). También
      están disponibles dos archivos en [este
      Drive](https://drive.google.com/drive/u/1/folders/1Bwh4_PpPlWTL3Lbz4O4fsIwnrXesXXFu),
      que incluye una versión TIF (quizá no es fácil de abrir en el
      teléfono) o KMZ (con Google Earth). Puedes usar el del aula
      también.
    - [Mapa topográfico (este enlace te lleva a un mapa muy detallado,
      sólo visible a escala 1:100,000 o mayor)](). Puedes usar el mapa
      3D del aula también.
    - Mapas de vegetación, o mapas de uso y cobertura. [Este
      enlace](https://biogeografia-master.github.io/medio-fisico-variables-ambientales/README.html)
      te lleva a la práctica anterior PA05; busca el mapa de PROBAV.
      También puedes intentar ver el de Medio Ambiente, usando [este
      informe](https://ambiente.gob.do/app/uploads/2016/12/uso-cobertura-suelo-2012.pdf)
      y el mapa propiamente en [este
      enlace](https://ambiente.gob.do/app/uploads/2016/12/Mapa_Uso_Cobertura_2012.pdf).
    - Carreteras, lugares poblados. Puedes usar OpenStreetMap o Google
      Maps.

3.  Identifica si hay áreas de concentración o ausencia de la especie, y
    toma nota de las características de esas áreas. Responde a las
    siguientes preguntas:

    - ¿Qué patrón de distribución presenta (e.g. agregado, etc.)?
    - ¿Dónde se encuentran la mayoría de los registros?
    - ¿Hay alguna relación visual con la información del medio físico o
      ambiental que tienes?
    - ¿Hay áreas donde no aparece el taxón, a pesar de que parecen tener
      condiciones similares a otras áreas con presencia?

Redacta un párrafo que sintetice la justificación de este paso, el
método empleado, qué obtuviste (describe los datos obtenidos) y qué
limitaciones encontraste.

------------------------------------------------------------------------

# **Ejercicio 2: Asociación con factores del medio físico**

Una vez hayas identificado la distribución espacial del taxón,
inspecciona si hay asociaciones claras con elementos del medio físico
como la geomorfología, elevación o tipos de suelo.

1.  Utiliza los mapas de aula para hacer una inspección visual de la
    distribución de la especie en relación con:
    - \*\*Latitud, longitud\*. ¿Se concentran los registros en
      determinadas porciones del país? ¿Está ausente el taxón en
      distintas porciones?
    - **Elevación**: ¿La especie se concentra en áreas montañosas,
      llanuras o zonas costeras?
    - **Topografía (como elevación y pendiente)**: ¿Parece haber una
      preferencia por áreas planas o inclinadas?
    - **Vegetación**: ¿Hay una coincidencia clara entre la presencia del
      taxón y ciertos tipos de vegetación (bosques, sabanas, etc.)?
    - **Lugares poblados, carreteras**. ¿Predominan los registros de
      presencia en lugares poblados y alrededor del viario?
    - **Otras variables que hayas considerado**. Evalúa asociación con
      otras variables.
2.  Responde a estas preguntas en función de lo que observes en los
    mapas. Anota cualquier patrón significativo, ya sea una fuerte
    asociación o la falta de ella.

Redacta un párrafo que sintetice la justificación de este paso, el
método empleado, qué obtuviste (describe los datos obtenidos) y qué
limitaciones encontraste.

------------------------------------------------------------------------

# **Ejercicio 3: Representación gráfica de patrones (en papel)**

Dibuja a mano un mapa de República Dominicana (vaya desafío, el talibán
aquí se quemaría) y marca en él las áreas donde observaste una mayor
presencia de tu taxón. También marca las áreas donde observaste una
ausencia, pero que crees que podrían tener condiciones favorables para
la especie.

1.  Usa tu mapa para identificar y destacar posibles patrones de
    distribución.
2.  Añade anotaciones que expliquen tus conclusiones.

------------------------------------------------------------------------

# **Ejercicio 4: Resumen estadístico básico (opcional)**

Si decides explorar un resumen estadístico sencillo de los registros de
presencia, puedes intentar crear una copia de cuaderno de ejemplo de
Acanthaceae de la PD02 en el servidor RStudio y aplicarlo a tu taxón.

Redacta un párrafo que sintetice la justificación de este paso, el
método empleado, qué obtuviste (describe los datos obtenidos) y qué
limitaciones encontraste.

Este ejercicio es opcional, y no se requiere para completar la práctica,
pero puedes usarlo para complementar tus observaciones visuales con
datos numéricos.

------------------------------------------------------------------------

# **Conclusión**

Escribe un resumen final de tus observaciones. Incluye: - Una reflexión
sobre los patrones espaciales observados. - Cualquier hipótesis que
puedas tener sobre las razones detrás de la distribución observada. - Si
encontraste o no una asociación clara con factores ambientales como la
elevación, pendiente o vegetación.

------------------------------------------------------------------------

# **Instrucciones adicionales**

1.  **Entrega:** Deberás entregar tu práctica en formato papel o
    “escaneada” con el teléfono, en cuyo caso un único archivo es
    preceptivo (e.g. PDF).

2.  **Formato:** Incluye todos los ejercicios solicitados, haciendo
    énfasis en la simple inspección visual (aun a riesgo de perder
    precisión) y las conclusiones sobre patrones espaciales.

3.  **Herramientas:** Utiliza los mapas provistos en el aula y cualquier
    material adicional que te parezca relevante.
