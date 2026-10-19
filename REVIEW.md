# Segunda revisión del manuscrito

Fecha: **19 de octubre de 2026**. Segunda lectura realizada por un proceso distinto del que redactó el libro, sobre la versión de autor con último commit `983c6e0`. Se revisaron **372 de 372 unidades**, incluidos los cuatro artículos promulgatorios, todos los preceptos operativos y los rangos derogados. No se trata de aprobación profesional externa ni de un dictamen para un caso concreto.

## Alcance y método real

Se leyeron por lotes el texto seleccionado de cada unidad y su comentario completo, examinando elementos, consecuencias, excepciones, ejemplos, remisiones, mezclas temporales y repeticiones. El [registro de lotes](second-pass-ledger.json) enumera todos los identificadores una vez. Se prestó atención especial a las capas históricas de mediación, banca, dependientes y pérdida de títulos; no se presentan sus órganos o procedimientos antiguos como una habilitación actual autosuficiente.

Se repitió la descarga oficial de metadatos y texto multiversión del BOE, con HTTP 200 y hash idéntico a las capturas de autor. La fecha técnica de actualización sigue siendo `20251216T102453Z`; la última publicación modificadora identificada es la Ley 11/2023, de 9 de mayo de 2023. Se leyó su art. 35 y la disposición final 18.6: entrada en vigor al año de publicación, 9 de mayo de 2024, para el cambio del art. 17. La fecha jurídica del libro se mantiene en 19 de octubre de 2026; la nueva descarga no se usa como prueba aislada de vigencia.

La enumeración independiente se rehízo a partir de los encabezamientos de clase `articulo` del HTML oficial nuevo, sin obtener los esperados de `units.jsonl` ni del tipo de bloque XML. Resultado: 372 identificadores únicos, igualdad de texto de las 372 unidades, 957 posiciones del Código (1–955, 38 bis y 43 bis) y cuatro artículos del decreto. Se comprobaron todas las cabeceras: no hay anexos ni disposiciones adicionales, finales o transitorias separadas. Los rangos derogados se conservan y los 445 bloques históricos caducados no se incorporan como derecho simultáneamente vigente. El HTML nuevo solo cambia el parámetro aleatorio de un script respecto de la captura anterior. [Evidencia de fuentes](second-pass-source-check.json), [cobertura](coverage-evidence.json), [descargas](sources/second-pass-verification.json).

## Hallazgos y correcciones

- **Art. 29:** se atribuía al texto una exigencia literal de euros; se distinguieron pesetas conservadas, presentación en euros (34.5) y moneda económica (38.h).
- **Art. 33:** los auxiliares corresponden al solicitante, con control judicial de forma y número; se corrigió su atribución al órgano judicial.
- **Arts. 43 y 48:** se precisaron 50 %, 10 % y seis meses para dispensa de subgrupo y 5 % para otras participaciones de memoria.
- **Art. 49:** se amplió el tratamiento de ámbito y reglas temporales, indicadores y materias, exención del subgrupo e informe separado. Se contrastó la disposición transitoria, apartado 3, de la Ley 11/2018, sin detenerse en el umbral histórico de 500 trabajadores.
- **Arts. 138 y 218:** se evitó limitar indebidamente el permiso a competencia y se corrigió la titularidad de fondos/firma sociales empleados para negocios propios.
- **Arts. 235 y 248:** se excluyó que una mera provisión autorice reparto y se distinguió la solicitud opcional de custodia judicial del deber de aviso/custodia del comisionista.
- **Arts. 334 y 339:** se explicitó la venta por número, peso o medida en el régimen de riesgo y se separaron perfección, fase de pago y vencimientos.
- **Art. 948:** se aclaró que la prescripción no interrumpida corre a favor del socio separado o excluido, evitando invertir el beneficiario.

El detalle estructurado consta en [review-result.json](review-result.json). Las correcciones se hicieron en los comentarios; no fue necesario alterar el texto legislativo ni rebajar el validador.

## Autoridades y remisiones externas

Se leyeron íntegramente las STC 113/1988 y 61/2010: encabezamiento, antecedentes, fundamentos y fallo. Se cotejaron con nuevas capturas oficiales los 17 y 13 párrafos de antecedentes/fundamentos respectivamente. En la primera, FJ 3–5 y fallo apoyan la garantía histórica de acceso al recurso, no un derecho ilimitado de examen. En la segunda, FJ 2 establece garantías de jurisdicción voluntaria y FJ 3–4 aplican diligencia de emplazamiento y retroacción en asunto sucesorio; no fija doctrina material de exhibición mercantil. No se confundieron las alegaciones de los litigantes con hechos o conclusiones del Tribunal. Se mantuvieron los límites históricos y temáticos de las [fichas](cases/TC-113-1988.md).

Se comprobaron directamente las versiones aplicables de los arts. 132–135 de la Ley 15/2015, 18 de la Ley 14/2013, 241 bis del texto refundido societario y 1 de la ley de usura; además, la disposición transitoria, apartado 3, de la Ley 11/2018 y la adicional 24 de la Ley 55/1999 con su entrada en vigor el 1 de octubre de 2000. Quedaron confirmadas las distinciones de nueve días para solicitar expediente, seis meses para rendimientos, un año para nuevos títulos y protección del tenedor de buena fe, sin confundirlas con las esperas históricas del Código. La búsqueda adicional del Supremo devolvió legislación y recopilación doctrinal, no una sentencia íntegra apta para añadir como autoridad: [registro](cases/search-log.json).

## Comprobaciones y límites

Se reconstruyó el libro con `build_repo.py` y se ejecutaron el validador estricto, la cobertura independiente, el cotejo HTML/XML, el control de 372 comentarios/delimitadores, el examen de repetición exacta y los enlaces locales. Los resultados finales se conservan en [validation.json](validation.json), [editorial-check.json](editorial-check.json) y [link-check.json](link-check.json). El validador final devolvió `ok: true`, literalidad `1.0`, 372 unidades y 275397 caracteres de comentario, sin errores ni advertencias. Ni longitud ni coincidencia automática sustituyen la lectura jurídica realizada.

La jurisprudencia sigue siendo selectiva y constitucional; no se afirma cobertura exhaustiva del Supremo. Tampoco se ofrece una investigación integral de toda legislación bancaria, laboral, concesional, internacional o de valores. El error HTTP 400 inicial de autor no conserva cuerpo, aunque sí todas las fuentes exitosas utilizadas. No quedan bloqueos materiales identificados para cerrar esta segunda lectura del alcance declarado. El resultado conserva estado de borrador revisado, sin aprobación externa, publicación ni envío.
