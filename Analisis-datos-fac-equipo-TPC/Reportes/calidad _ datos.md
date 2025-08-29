# Informe sobre calidad de datos

## Introduccion

El presente informe tiene como objetivo analizar la información recopilada en la encuesta JEFAB 2024, aplicada a un total de 6.423 participantes pertenecientes a la Fuerza Aérea Colombiana y su núcleo familiar. El instrumento recoge datos de carácter sociodemográfico, familiar, educativo, social y habitacional, con el fin de identificar condiciones de vida, dinámicas de convivencia, redes de apoyo y factores de bienestar que impactan directamente en la calidad de vida de los encuestados.

Este análisis busca ofrecer una visión integral de la población, destacando sus principales características, fortalezas y situaciones de vulnerabilidad. De esta manera, se generan insumos que permiten orientar la formulación de estrategias, programas y políticas institucionales en beneficio del personal y sus familias, promoviendo su desarrollo social, familiar y comunitario.

Alguna de las variables hablan sobre:

Datos sociodemográficos: sexo, género, edad, estrato, nivel educativo.

Información familiar: estado civil, número de hijos, relación con padres y hermanos, dinámicas familiares.

Aspectos de vivienda: si es propia, en arriendo, número de personas en el hogar.

Situaciones especiales: discapacidad, fallecimientos en la familia, violencia intrafamiliar.

## Problemas con la base de datos

### Base de datos sin contextualización 

La empresa no da contexto sobre los datos, por lo que la ivestigación sobre esta retrasa la entrega de la base de datos limpiada, corregida y con las variables que los expertos dicen.

### Datos faltantes

1. Descripción del problema

Durante la exploración de la base de datos se evidenció que un número significativo de variables presenta más del 50% de información faltante. Esta situación se debe principalmente a dos motivos:

Variables no aplicables: en ciertos casos la pregunta no es relevante para todos los encuestados (por ejemplo, datos que solo se responden si la persona tiene hijos o pareja).

No respuesta voluntaria: en otras ocasiones, el encuestado optó por no suministrar la información solicitada.

2. Impacto del problema

Limitaciones en el análisis: las variables con alta proporción de valores perdidos reducen su utilidad para generar conclusiones confiables.

Posible sesgo: la falta de respuesta no siempre es aleatoria; en algunos casos puede reflejar resistencia a compartir información sensible, lo cual introduce un sesgo en los resultados.

Dificultad para la imputación: cuando la ausencia supera el 50%, los métodos de imputación dejan de ser recomendables, ya que el valor generado no representaría fielmente la realidad.

3. Recomendaciones y en el proceso realizado 

No imputar variables con más del 50% de datos faltantes, ya que esto comprometería la validez de los análisis.

Utilizar únicamente las variables con suficiente información para los análisis descriptivos y predictivos, priorizando aquellas con niveles aceptables de completitud.

Reportar de manera explícita las limitaciones derivadas de la ausencia de información, tal como se ejemplifica en el documento “Faltantes_python_personal” de la carpeta “Reportes”.

### Problemas de Codificación de Caracteres

1. Descripción del problema

Al revisar el archivo se identificaron errores de codificación en los textos, específicamente en aquellos que contienen letras con tilde (á, é, í, ó, ú) y la letra “ñ”. Estos caracteres aparecen representados de forma incorrecta, generando palabras con símbolos extraños.

Ejemplos encontrados:

La palabra “TECNOLÓGICO” aparece como “TECNOLOGÃ“GICO”.

La palabra “TÉCNICO” aparece como “TÃ‰CNICO”.

La frase “SEGURIDAD Y DEFENSA DE BASES AÉREAS” aparece como “SEGURIDAD Y DEFENSA DE BASES AÃ‰REAS”.


2. Impacto del problema

Claridad de la información: los errores dificultan la comprensión de los datos y pueden generar confusión.

Calidad del análisis: al existir palabras escritas de manera diferente por error de codificación, estas pueden interpretarse como categorías distintas cuando en realidad son la misma.

Presentación de resultados: los reportes y visualizaciones pierden calidad y profesionalismo si contienen textos mal codificados.

3.  Recomendaciones y en el proceso realizado 

Revisar y limpiar las categorías afectadas, de modo que los términos queden uniformes y no se dupliquen por errores de escritura.

Adoptar como práctica institucional la verificación del encoding al momento de almacenar y compartir bases de datos para evitar recurrencia del problema.

### Inconsistencias en la Base de Datos

Durante la revisión de la base de datos se identificaron inconsistencias en algunas respuestas, particularmente en variables relacionadas entre sí. Un ejemplo claro es cuando el número total de hijos reportado resulta ser menor que el número de hijos que habitan en el hogar, lo cual no es coherente.

Estas inconsistencias fueron advertidas a la experta responsable, quien fue informada sobre los posibles impactos en el análisis. Finalmente, se determinó que la decisión sobre cómo manejar estas situaciones recaería en ella, mientras que el trabajo de depuración se mantuvo en la identificación y señalamiento de los casos problemáticos.

## Conclusión

La base de datos resultó difícil de utilizar debido a los problemas previamente señalados: presencia de errores de codificación de caracteres, alta proporción de datos faltantes en ciertas variables y falta de respuesta por parte de la empresa para aclarar inconsistencias. Estos factores generaron retrasos en el proceso de limpieza y depuración de la información.

A pesar de ello, se tomó la decisión de no imputar los valores faltantes, ya que en algunas variables más del 50% de los datos no estaba disponible y su reemplazo comprometería la calidad del análisis. En este sentido, se determinó que trabajar con el 92% de las observaciones completas es adecuado y suficiente para garantizar la validez de los resultados, manteniendo la integridad metodológica del estudio.

