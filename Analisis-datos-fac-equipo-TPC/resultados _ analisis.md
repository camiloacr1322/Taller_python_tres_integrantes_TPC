# Resultados de los tres integrantes del grupo

Base de datos de la Fuerza Aérea Colombiana.

## Calidad de datos 

###  ¿Qué columnas tienen más datos faltantes?

| #variable | Columna                               | #Datos_Faltantes | Porcentaje |
|-----------|---------------------------------------|------------------|------------|
| 213       | NUMERO_PERSONAS_APORTE_SOSTENIMIENTO2 | 3928             | 61.155223  |
| 212       | NUMERO_HABITAN_VIVIENDA2              | 3808             | 59.286938  |
| 31        | NUMERO_HIJOS                          | 3217             | 50.085630  |
| 32        | HIJOS_EN_HOGAR                        | 3200             | 49.820956  |


Son cuatro las columnas con más faltantes, cada una con el 49% o más haciendo dificil la imputaciòn de estas variables, aunque en algunas variables se arregla el problema de otra manera, explicación más detallada en la parte dos de "Faltantes_python_personal" en la carpeta de "Reportes"

### ¿Hay registros duplicados?

No se encuentran registors duplicados, esto se muestra en el archivo "datos_exploración" en la carpeta "Analisis-datos-fac-equipo-TPC" o "Faltantes_python_personal" en la carpeta "Reportes"


### ¿Qué problemas de encoding se detectan?

| Texto con fallo            | Texto correcto            |
|-----------------------------|---------------------------|
| TECNOLOGÃ“GICO              | TECNOLÓGICO               |
| TÃ‰CNICO                    | TÉCNICO                   |
| SEGURIDAD Y DEFENSA DE BASES AÃ‰REAS | SEGURIDAD Y DEFENSA DE BASES AÉREAS |

Cuando abrimos la base de datos, algunos textos con tildes (á, é, í, ó, ú) o con la letra ñ aparecen con símbolos extraños, como “TECNOLOGÃ“GICO” en vez de “TECNOLÓGICO”.

Este tipo de error es común en bases grandes y afecta la claridad de la información, ya que puede generar categorías duplicadas o confusión en los reportes. Por ejemplo, “TÉCNICO” y “TÃ‰CNICO” se interpretarían como dos valores distintos, aunque en realidad sean lo mismo. 

Si desea ver la solución o tener más detalle esto se enceuntra en el archivo "datos_exploración" en la carpeta "Analisis-datos-fac-equipo-TPC" o "Faltantes_python_personal" en la carpeta "Reportes"


## Análisis demográfico

### Distribución por Sexo

Hombres: 4127 (69.6%)
Mujeres: 1804 (30.4%)

La muestra evidencia una clara predominancia masculina, lo cual resulta coherente con el contexto militar de la Fuerza Aérea Colombiana. No obstante, la participación femenina también es significativa, pues representa cerca de un tercio de la población analizada. Este balance refleja los avances en inclusión y diversidad dentro de la institución, aunque aún persiste una diferencia marcada en la proporción.

<img width="709" height="547" alt="image" src="https://github.com/user-attachments/assets/4f5f129c-1b2d-4046-8ddb-0b5aaf404407" />
