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

La pirámide poblacional refleja una marcada diferencia en la participación de hombres y mujeres dentro de la muestra. Se observa que los hombres representan la mayoría en todos los rangos etarios, especialmente en los grupos de 28–32 y 33–37 años, donde la brecha entre géneros es más evidente. Aunque las mujeres están presentes en todos los intervalos de edad, su participación es considerablemente menor, lo que coincide con la distribución general de la muestra en la que predominan los hombres. Esta diferencia resalta la composición demográfica característica de un contexto militar, donde históricamente la presencia masculina ha sido mayoritaria.

<img width="695" height="497" alt="image" src="https://github.com/user-attachments/assets/ac66b405-4c80-4674-a573-63a55c9767a4" />

El índice de masculinidad muestra una clara predominancia de hombres frente a mujeres en la mayoría de los rangos de edad, superando ampliamente el umbral de 100 (equilibrio). La diferencia es más marcada entre los 18 y 42 años, donde por cada 100 mujeres hay entre 250 y 300 hombres aproximadamente. A partir de los 43 años la brecha comienza a disminuir, aunque nunca se iguala, y en el rango de 63–67 años se observa un pico atípico de masculinidad. Esto confirma el sesgo de género presente en la muestra y la mayor participación masculina en el contexto militar.

<img width="704" height="513" alt="image" src="https://github.com/user-attachments/assets/f5727c63-6f40-4b9b-9fe4-1829ce973e2c" />

<img width="859" height="591" alt="image" src="https://github.com/user-attachments/assets/b3c5c65a-1cee-4d7e-9ef3-832624ded302" />

El análisis de la frecuencia de grados militares muestra que la mayor concentración de individuos se encuentra en el rango de suboficiales, con un total de 2.508 casos. Este valor supera ampliamente al de los oficiales (1.755) y civiles (1.668), lo que refleja una estructura jerárquica donde predomina el personal subalterno frente a las demás categorías.

Al desagregar los datos por género, se observa que en todas las categorías la participación masculina es predominante. La diferencia es especialmente notoria en el rango de suboficiales, donde los hombres superan de manera considerable a las mujeres, mientras que en la categoría civil la brecha es mucho menor. Este comportamiento evidencia una marcada desigualdad de género en la composición de los grados militares, aunque con una mayor presencia relativa de mujeres en los cargos civiles.



## Anàlisis Familiar

### ¿Qué porcentaje del personal está casado?

El **58.76%** del personal encuestado está casado.  
Esto indica que la mayoría del personal de la FAC tiene vínculos familiares formales, lo cual puede influir en sus dinámicas de convivencia, necesidades familiares y bienestar emocional.  

---

### ¿Cuántos tienen hijos y cuántos viven con ellos?

**3181 personas** tienen hijos.De ellas, **2706 personas** viven con sus hijos.  
La gran mayoría de quienes tienen hijos conviven con ellos, lo que sugiere una estructura familiar activa y presente. 

---

### ¿Hay relación entre edad y estado civil?

Sí, hay una relación clara.  
  - **Solteros/as**: edad promedio de **30 años**.  
  - **Casados**: **39 años**.  
  - **Separados/divorciados**: entre **40 y 41 años**.  
  - **Viudos/as**: **47 años**.  

La edad está directamente relacionada con el estado civil. A medida que aumenta la edad, es más probable que las personas estén casadas, separadas o viudas.
