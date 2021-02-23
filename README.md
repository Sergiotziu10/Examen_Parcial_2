# Examen_Parcial_2

- Primero se tendra que importar Panda.

import pandas as pd

- Seguidamente definimos una variable, para abrir el archivo directamente en un DataFrame utilizaremos
  el comando pd.read_csv, porteriormente dentro de los parentesis llevara unas comillas para indicar la
  ruta de dicho archivo con la extensión .CSV.
  
df = pd.read_csv('Examen/data_by_artist.csv')

- En mi caso para poder desplazarme facilmente, use el comando .info() para que devuelva información como
  (número de filas, número de columnas, índices, tipo de las columnas y memoria usado). La df es varible.
  
df.info()

- El siguiente comando "variable.head(10)" Lee las primeras 10 líneas de la tabla de artistas. si queremos que lea las 10 ultimas
  tendremos que insertar el comando "variable.tail(10)".

df.head(10)
df.tail(10)

- los posibles datos que puedan relacionarse pienso que son "varible.describe()" que es un metodo que devuelve
  información estadística de los datos del dataframe o de la serie o bien devuelve un dataframe, y el "variable.artists.count()"
  sirve para poder contar cuando informacion existe en una columna especifica en mi caso fue la columna Artistas.

df.describe()
df.artists.count()
