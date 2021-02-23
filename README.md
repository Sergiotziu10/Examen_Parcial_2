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

- 
