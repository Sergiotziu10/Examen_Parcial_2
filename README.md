# Examen_Parcial_2

- Primero se tendrá que importar Panda.

      import pandas as pd

- Seguidamente definimos una variable, para abrir el archivo directamente en un DataFrame utilizaremos el comando pd.read_csv, posteriormente dentro de los paréntesis llevara unas comillas para indicar la ruta de dicho archivo con la extensión .CSV.
  
      df = pd.read_csv('Examen/data_by_artist.csv')

- En mi caso para poder desplazarme fácilmente, use el comando .info() para que devuelva información como (número de filas, número de columnas, índices, tipo de las columnas y memoria usado). La df es variable.
  
      df.info()

- El siguiente comando "variable.head(10)" Lee las primeras 10 líneas de la tabla de artistas. si queremos que lea las 10 últimas tendremos que insertar el comando "variable.tail(10)".

      df = df.head(10).sort_values(by='artists', ascending=True)
      df['artists']
      

- Los posibles datos que puedan relacionarse pienso que son "varible.describe()" que es un método que devuelve información estadística de los datos del dataframe o de la serie o bien devuelve un dataframe, y el "variable.artists.count()" sirve para poder contar cuando información existe en una columna especifica en mi caso fue la columna Artistas.

      df.describe()
      df.artists.count()


- Para identificar las variables de Media se usó el comando "media = df.mean()", si se quiere una columna en especifica "media = df.['columna']mean()" en este caso donde está la palabra energy puede ser otra columna, saca la media de una columna deseada.

      media = df.mean()
      print (media)
  
- Para identificar las variables de la Mediana se usó el comando "mediana = df.median()", si se quiere una columna en especifica "mediana = df['columna'].median()"  en este caso donde está la palabra energy puede ser otra columna, relación a la mediana de una columna.

      mediana = df.median()
      print (mediana)
  
- Para identificar las variables de la Varianza se usó el comando "varianza = df["columna"].var()", si se quiere una columna en especifica "varianza = df['columna'].var()" en este caso donde está la palabra energy puede ser otra columna, calcula la varianza de una columna.

      varianza = df.var()
      print (varianza)
  
- Para identificar las variables del máximo se usó el comando "máximo = df.max()", si se quiere una columna en especifica "máximo = df["columna"].max()" en este caso donde está la palabra energy puede ser otra columna, indica el valor máximo de una columna.

      maximo = df.max()
      print (maximo)

- Para identificar las variables del mínimo se usó el comando "mínimo = df.min()", si se quiere una columna en especifica "mínimo = df["columna"].min()" en este caso donde está la palabra energy puede ser otra columna, indica un valor mínimo de una columna.             

      minimo = df.min()
      print (minimo)
      
- Método estadístico que trata de modelar la relación entre una variable continua y una o más variables independientes mediante el ajuste de una ecuación lineal. en este caso se uso el comando
