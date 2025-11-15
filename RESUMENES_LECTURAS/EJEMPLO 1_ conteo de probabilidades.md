En una bolsa con cuatro canicas de do colores: azul y blanco.
Pero nos e sabe cuantas hay de cada color.
Sabemos que hay 5 posibilidades, de las cuales son las unicas consistentes con lo que sabemos que hay en la bolsa. LLamamos estas posibilidades conjeturas.
![[Pasted image 20251114180450.png]]
La meta es saber cual es la más plausible. Se tiene la evidencia de una secuencia de tres maras las cuales se fueron sacando una por una siendo devuelta y sacudiendo de nuevo la bolsaantes de sacar la siguiente. 
La secuencia es :
![[Pasted image 20251114180934.png]]
Creando asi la primera posibilidad siguiendo la conjetura de :
![[Pasted image 20251114181031.png]]
Visualizamos las posibilidades:
![[Pasted image 20251114181107.png]]
Solo se registro el color d elas canicas, significando que hay tres maneras de ver. Al sacar or¿tra canica se expande las posibilidades:
![[Pasted image 20251114181941.png]]
ahora hay 16 posibilidades, una por cada par.
Por se tiene el supuesto que al sacudir la bolsa cada canica tiene la misma probabilidad de ser sacada independiente de la anterior.
Generando 64 caminos posibles, pero considerando la extracción de la bolsa algunos son elminados por logica.
Si se imaginan los datos reales trazando un camino de be haber pasado primero por el azul cercano al origen. 
La segunda extracción es blanca creando tres caminos bifurcados en la canica azul; ya que solo se resgistro el color y no el orden se sabe que a medida que pasan los datos paso por algun blanco.
La tercera extracción es azul, por lo que se deduce que los tres caminos de la capa intermedia contienen un camino azul, dejando tres maneras de la secuencia.
![[Pasted image 20251114183149.png]]
Asi solo quedn los caminos que segun la logica son por los que pasaron, pero no se sabe cual de los tres fue por el que paso los datos; siguiendo con la posibilidad de la bolsa con una caninca zul y tres blancas, ya que son los unicos consistentes con el contenido de la bolsa.
Demostrando que 3 de 64 son las maneras que la bolsa contiene la secuencia. ![[Pasted image 20251114183501.png]]
Pero la inferencia compara el conteno con el número de maneras de cada una de las otras conjeturas. 
Eliminando asi las conjeturas logicas que son incompatibles con los datos.
![[Pasted image 20251114183705.png]]
![[Pasted image 20251114183717.png]]
Ahora se muestran tres conjeturas, de todas las maneras que cada unas podria producir los datos observados:
![[Pasted image 20251114183842.png]]
![[Pasted image 20251114183851.png]]
![[Pasted image 20251114183902.png]]
Considerando 5 conjeturas diferentes y se cntaron cuantas secuencoas podrian producir los datos observados:
![[Pasted image 20251114184948.png]]
Calculandose al contar el número de caminos en cada anillo y multiplocando por los conteos. Sien aun un conteo de caminos logicamente posibles. 
Demanera que se obtiene lo mismo que al graficar los conteos:
![[Pasted image 20251114185950.png]]
Al comparar tenemos se obtiene parte de la evaluación de plausibilidad relativa de la composición de la bolsa. Pero para comparar se necesita contar las maneras de realizar cada conjetura.  
Cuando no se tienen motivos para lo contrario  considerar ambas conjeturas plausibles y comparar los recuentos de manera directa.

La primera justificación de usar el número de caminos en el jardin como medida de plausibilidad relativa es lógica, 
