Laboratorio | Limpieza y discusión de datos.
Para esta práctica de laboratorio, usaremos el mismo conjunto de datos que usamos en las prácticas de laboratorio anteriores. Recomendamos usar el mismo cuaderno, ya que reutilizará las mismas variables que creó y usó anteriormente en los laboratorios.

Instrucciones
Hasta ahora hemos trabajado en EDA. Esta práctica de laboratorio se centrará en la limpieza y discusión de datos de todo lo que notamos antes.

Comenzaremos eliminando los valores atípicos. Hasta ahora, hemos analizado diferentes métodos para eliminar valores atípicos. Utilice el que le resulte más cómodo y defina una función para ello. Utilice la función para eliminar los valores atípicos y aplicarlos al marco de datos.
Cree una copia del marco de datos para la manipulación de datos.
Normalizar las variables continuas. Puede utilizar cualquier método que desee.
Codificar las variables categóricas.
La variable tiempo puede resultar útil. Intente transformar sus datos en datos útiles. Sugerencia: Puede resultar útil utilizar el día, la semana y el mes como números enteros.
Dado que el modelo solo aceptará datos numéricos, verifique y asegúrese de que cada columna sea numérica; si algunas no lo son, cámbielas mediante codificación.
Sugerencia para variables categóricas

Debe tratar las variables categóricas como se muestra a continuación (para la codificación ordinal, también se proporciona un código ficticio):
# One hot to state
# Ordinal to coverage
# Ordinal to employmentstatus
# Ordinal to location code
# One hot to marital status
# One hot to policy type
# One hot to policy
# One hot to renew offercustomer_df
# One hot to sales channel
# One hot vehicle class
# Ordinal vehicle size

data["coverage"] = data["coverage"].map({"Basic" : 0, "Extended" : 1, "Premium" : 2})
# given that column "coverage" in the dataframe "data" has three categories:
# "basic", "extended", and "premium" and values are to be represented in the same order.
