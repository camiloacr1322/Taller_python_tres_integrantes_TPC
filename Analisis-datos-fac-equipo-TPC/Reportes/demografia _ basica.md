 # Análisis Demográfico Básico

Este proyecto realiza un **análisis demográfico básico** a partir de una base de datos .  
El trabajo se desarrolló en **Google Colab**, cargando los datos desde Google Drive y generando distintos gráficos para responder preguntas demográficas básicas.

---

## Pasos realizados

### 1. Importación de librerías y carga de datos
Se importaron las librerías necesarias y se cargó la base en un `DataFrame`.  
**Importante** porque es el punto de partida para manipular y analizar la información disponible.

---

### 2. Revisión de la variable sexo
Se verificó que la variable `SEXO` contuviera únicamente dos categorías: **hombre** y **mujer**.  
**Importante** porque asegura consistencia en el análisis de género y evita errores derivados de valores duplicados o mal escritos.

---

### 3. Distribución de edades (Histograma)
Se construyó un histograma para visualizar cómo se distribuyen las edades en la base de datos.  
**Porque**  permite identificar si la población es principalmente joven, adulta o envejecida, lo cual es clave en estudios poblacionales.

---

### 4. Creación de rangos etarios
Se agruparon las edades en intervalos de 5 y 10 años para formar los **rangos etarios**.  
**Importante** porque los rangos etarios son la base de análisis demográficos comparativos y permiten construir indicadores como la pirámide poblacional.

---

### 5. Pirámide poblacional
Se construyó la pirámide poblacional con hombres representados en el lado izquierdo y mujeres en el derecho.  
**Porque**  es el gráfico central de la demografía: muestra la distribución de la población por edad y sexo, facilitando el análisis de estructura y tendencias poblacionales.

---

### 6. Índice de masculinidad
Se calculó el número de **hombres por cada 100 mujeres** en cada rango de edad.  
**Importante** porque permite identificar desequilibrios en la relación de géneros, observando si hay más hombres o más mujeres en determinados grupos etarios.

---

### 7. Frecuencia de categorías militares (conteo total)
Se analizó la frecuencia de la variable `categoria`, que representa el grado militar, mediante un gráfico de barras con la cantidad de registros en cada categoría.  
**porque**  permite identificar cuál es el grado militar más frecuente dentro de la base.

---

### 8. Frecuencia de categorías militares por género
Se construyó un gráfico segmentado por género para observar cómo se distribuyen los grados militares entre hombres y mujeres.  
**Importante** porque permite analizar las diferencias en la representación de género dentro de las categorías militares.

---

## Conclusiones

- Se obtuvo una **visión general de la población** en términos de edad y género.  
- Se identificaron **diferencias en la distribución por sexo** a través de la pirámide poblacional y el índice de masculinidad.  
- Se determinó cuál es el **grado militar más frecuente** en la base de datos.  
- Se exploraron las **diferencias por género en las categorías militares**, lo que aporta a un entendimiento más profundo de la estructura poblacional.  

Este análisis constituye un **primer diagnóstico demográfico** que puede servir como base para estudios más avanzados en estructura social, familia y dinámicas poblacionales.
