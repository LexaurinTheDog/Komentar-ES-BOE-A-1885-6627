# Fuentes y evidencia

Comprobación realizada el **19 de octubre de 2026**. El [manifiesto JSON](sources/verification.json) conserva URL exacta, acceso, HTTP, tamaño, SHA-256 y verificación de formato. Las respuestas XML contienen datos normativos y los HTML, el código o decisión esperados; no se aceptaron páginas antibot como fuentes legislativas. Una primera petición de API sin encabezado Accept recibió 400; la repetición correcta con `application/xml` recibió 200 y se conserva íntegra. El cuerpo inicial de error no fue conservado y no se usa como evidencia de texto.

| Fuente oficial | Evidencia local | Uso efectivo |
| --- | --- | --- |
| [Código de Comercio, ficha actual](https://www.boe.es/buscar/act.php?id=BOE-A-1885-6627) | [HTML](sources/boe-current.html), [XML](sources/boe-api.xml), [metadatos](sources/metadata.xml) | Texto, estructura, versiones, caducidades y análisis de reformas |
| [Ley 11/2023](https://www.boe.es/diario_boe/txt.php?id=BOE-A-2023-11022) | [Publicación XML](sources/reform-2023.xml) | Art. 35 y disposición final 18.6: art. 17 eficaz desde 9 de mayo de 2024 |
| [Ley 11/2018](https://www.boe.es/diario_boe/txt.php?id=BOE-A-2018-17989) | [Publicación XML](sources/law11-2018.xml) | Extensión de información no financiera de su disposición transitoria.3 |
| [Ley 55/1999](https://www.boe.es/diario_boe/txt.php?id=BOE-A-1999-24786) | [Publicación XML](sources/law55-1999.xml) | Disposición adicional 24: integración de notarios y corredores, eficaz desde 1 de octubre de 2000 |
| [Ley 15/2015](https://www.boe.es/buscar/act.php?id=BOE-A-2015-7391) | [XML multiversión](sources/jurisdiccion-voluntaria.xml) | Arts. 132–135, versión efectiva a fecha de referencia; art. 134.2 reformado desde 20 de marzo de 2024 |
| [Ley de Sociedades de Capital](https://www.boe.es/buscar/act.php?id=BOE-A-2010-10544) | [XML](sources/sociedades-capital.xml) | Art. 241 bis: acción social o individual, plazo desde posibilidad de ejercicio |
| [Ley 14/2013](https://www.boe.es/buscar/act.php?id=BOE-A-2013-10074) | [XML](sources/emprendedores.xml) | Art. 18: legalización telemática y control formal |
| [Ley de 23 de julio de 1908](https://www.boe.es/buscar/act.php?id=BOE-A-1908-5579) | [XML](sources/usura.xml) | Art. 1: límites de usura frente a lectura aislada del art. 315 |
| [STC 113/1988](https://hj.tribunalconstitucional.es/es/Resolucion/Show/1054) | [Ficha](cases/TC-113-1988.md), [HTML completo](sources/tc113-1988.html) | Garantía procesal histórica del recurso; no interpretación vigente exhaustiva de exhibición |
| [STC 61/2010](https://hj.tribunalconstitucional.es/es/Resolucion/Show/6700) | [Ficha](cases/TC-61-2010.md), [HTML completo](sources/tc61-2010.html) | Garantías constitucionales también en jurisdicción voluntaria; asunto sucesorio |

El [registro jurisprudencial](cases/search-log.json) declara consultas, exclusiones y límites. No se incorpora una decisión del Tribunal Supremo a partir de un resultado de buscador. Para las unidades técnicas y derogadas no se seleccionó una autoridad judicial suficientemente relevante y verificada; ello no es una afirmación de inexistencia. Las dos fichas constitucionales contienen su alcance real y no justifican afirmar cobertura jurisprudencial sustantiva integral del Código.

La [selección temporal](sources/selection.json), el [mapa de cambios](sources/change-map.json), la [cobertura completa](coverage-evidence.json), el [informe resumido](completeness-report.json) y la [comparación HTML/XML](html-text-agreement.json) permiten reproducir el tratamiento del texto. Se preserva el [intake](sources/intake-20261002.md), cuyo hash coincide con el comunicado en la asignación. Los cambios de formato y exclusión histórica no se presentan como nuevas reformas posteriores al intake.

No se ha investigado exhaustivamente todo el derecho bancario, laboral, concesional, de mercados o internacional al que remiten las reglas antiguas. En esos puntos se explican presupuestos y se declara necesidad de coordinación, sin atribuir una solución sectorial completa a la literalidad del Código. Tampoco se emite opinión individualizada sobre un litigio.
