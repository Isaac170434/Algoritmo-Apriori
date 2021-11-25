# Algoritmo Apriori
Repositorio creado para el desarrollo del algoritmo Apriori
##### Por: Antony Isaac Huaman Hermoza

## Contenido

```
├── 1. Implementar el algoritmo Apriori
├── 2. Aplicar el algoritmo y obtener reglas de asociación
└── 3. Explicar las reglas obtenidas
```

## Requerimientos

Son las librerías requeridas para ejecutar esta tarea. Los requerimientos se pueden instalar fácilmente con:

| Libreria          | 
| ----------------- |
| `altair==2.2.2`   |
| `pandas==0.23.4`  |
| `numpy==1.15.1`   |

| Archivo           | 
| ----------------- |
| `spotify.npy`     |

## Ejecución del archivo

Para ejecutar el *notebook (Jupyter)*:

1. Tener instaladas las librerías requeridas (Requerimientos)
2. Abrir aplicación de anaconda y seleccionar la opción de `jupyter notebook`.
3. En la ventana del navegador que se abrirán todos los archivos, buscar la carpeta del proyecto y hacer click sobre `Algoritmo–Apriori.ipynb`.

## Descripción del contenido:

### 1. Implementación del algoritmo Apriori

Implementación del algoritmo. Para estructurar mejor el código, se implementarán las siguientes funciones:

  • get_frequent_itemsets(playlists, min_support): Recibe la esctructura de datos que contiene a las playlists y retorna una estructura con los itemsets frecuentes, bajo un umbral mínimo de confianza.
  • generate_association_rules(frequent_itemsets, confidence = 0, lift = 0): Recibe los itemsets frecuentes generados por la función anterior y retorna las reglas de asociación. Se le puede entregar umbrales de confianza o lift para las reglas que se retornarán. Por ejemplo, si se llama esta función con los ar- gumentos confidence = 0.5 y lift = 1.2, se espera que se retornen aquellas reglas que cumplan con una confianza ≥ 0.5 y un lift ≥ 1.2.

### 2. Aplicar el algoritmo y obtener reglas de asociación

Aplicación del algoritmo implementado en la base de datos `spotify.npy`, filtrando las
mejores 10 reglas de asociación de acuerdo criterios de calidad.

### 3. Explicar las reglas obtenidas

Selección de 4 reglas y comentando su calidad de acuerdo a los diferentes indicadores disponibles (support, confidence y lift). Interpretación de las reglas según el género y/o el artista de las canciones (que puedes buscar según el nombre de la canción).
