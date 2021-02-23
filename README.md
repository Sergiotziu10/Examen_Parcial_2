# Examen_Parcial_2

- Primero se tendra que importar Panda.

***import pandas as pd***

- Seguidamente definimos una variable, para abrir el archivo directamente en un DataFrame utilizaremos
  el comando pd.read_csv, porteriormente dentro de los parentesis llevara unas comillas para indicar la
  ruta de dicho archivo con la extensión .CSV.
  
***df = pd.read_csv('Examen/data_by_artist.csv')***

- En mi caso para poder desplazarme facilmente, use el comando .info() para que devuelva información como
  (número de filas, número de columnas, índices, tipo de las columnas y memoria usado). La df es varible.
  
***df.info()***

- El siguiente comando "variable.head(10)" Lee las primeras 10 líneas de la tabla de artistas. si queremos que lea las 10 ultimas
  tendremos que insertar el comando "variable.tail(10)".

***df.head(10)***

***df.tail(10)***

- Los posibles datos que puedan relacionarse pienso que son "varible.describe()" que es un metodo que devuelve
  información estadística de los datos del dataframe o de la serie o bien devuelve un dataframe, y el "variable.artists.count()"
  sirve para poder contar cuando informacion existe en una columna especifica en mi caso fue la columna Artistas.

***df.describe()***

***df.artists.count()***


- Para identificar las variables de Media se uso el comando "media = df["energy"].mean()" en este caso donde esta la palabra energy
  puede ser otra columna, saca la media de una columna deseada.
  
- Para identificar las variables de la Mediana se uso el comando "mediana = df["energy"].median()" en este caso donde esta la palabra energy
  puede ser otra columna, relacion el promedio de una columna.
  
- Para identificar las variables de la Varianza se uso el comando "varianza = df["energy"].var()" en este caso donde esta la palabra energy
  puede ser otra columna, calcula la varianza de una columna.
  
- Para identificar las variables de la maximo se uso el comando "maximo = df["energy"].max()" en este caso donde esta la palabra energy
  puede ser otra columna, indica el valor maximo de una columna.

- Para identificar las variables de la minimo se uso el comando "minimo = df["energy"].min()" en este caso donde esta la palabra energy
  puede ser otra columna, indica un valor minimo de una columna.
  
***media = df["energy"].mean()***

media

***mediana = df["energy"].median()***

mediana

***varianza = df["energy"].var()***

varianza

***maximo = df["energy"].max()***

maximo

***minimo = df["energy"].min()***

minimo
