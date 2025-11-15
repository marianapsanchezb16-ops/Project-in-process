El principal interés es la estadística en la ciencia y como esta motiva el razonamiento estadístico y como se conecta al data.

Se usan tres componentes principales
Para modelos estadísticos los cuales procesan data y produce estimados (conocimiento científico) requiere modelos científicos adicionales (causal).
La razon para análisis estadísticos no se encuentra en los datos mismos, sino en las causas de los datos.
Las causas de los datos no se pueden extraer de los datos. Sin causas de entrada, no hay causas de salida.

### Inferencia causal
Solo hay un moderado causal con un nivel de abstracción.
- Más que la coordinación de variables.
- Predicción de intervención(ausencia de intervención, consecuencia de cambio de variable en otras variables)
- Imputación de observaciones perdidas.
==Correlación no implica causación== 
- Correlación es una medida limitada de asociación.
- Las variables se pueden asociar pero no tienen correlación.
- Las asociaciones son bidireccionales:
    - No causación
    - Solo medidas estadísticas

### Predicción causal
Conocer una causa significa ser capaz de predecir las consecuencias de una intervención.
==Que pasa si hago esto?==
### Imputación causal
Conocerla una causa es ser capaz de construir resultados contrafácticos no observados.
==Y si hubiera hecho algo diferente?==
### Causas no son opcionales
Cuando la meta es descriptiva, requiere un modelo causal.


---
## DAG
- Gráfico directo acílico
- Modelo causal heurístico
- Clarifica pensamiento científico
- Analiza y deduce apropiadamente los modelos estadísticos
==Qué podemos decidir, sin suposiciones adicionales==
Son bastante abstractos en los modelos causales
![[Pasted image 20251109151620.png | 400]]
- El nombre de las variables -> letras
- Relaciones causales -> flechas
    Si cambia una variable al inicio de la flecha cambiara también la variable del final pero no alreves.

Asume 
     ->Lineales
     Todas interaccionan
La relación X~Y, siendo:
    X -> tratamiento 
    Y -> resultado
    A ->Influencia del tratamiento
    C ->Causas comunes (variable a controlar)
    B -> Causas de competencia 
- Se pueden realizar multiples preguntas
- Cada causa necesita un modelo diferente/procedimiento estadístico
- Variables de control:
    - Buenas -> Ayuda a influenciar y corregir la causa.
    - Malas -> Variables que crean confusión en los modelos.
- Bombas de intuición -> en la cabeza del investigador que lo saca de los números y en la creencia para tener sentido.

---
## PRAGA
- Se le llama Golems a los modelos estadísticos -> solo ejecuta las instrucciones
- Rabbi Löw (1512-1609)
- Son robots creados para resolver una tarea especifica 
- Programas computacionales -> corren en arcilla o silicona
- Los procedimientos son únicamente Bayesianos con el objetivo de rechazar las hipótesis nulas.
- El t-test creado por William Seeley Gossett-> Creado para realizar test en un pequeño lote de Guinnes (cerveza).
![[Pasted image 20251109162405.png|500]]
---
## Modelos nulos raramente únicos
Se diseñan multiples modelos y analizan sus implicaciones. 
![[Pasted image 20251109162743.png | 500]]
- Si la evolución es neutra la selección no influye, se necesitara crear otras suposiciones com el tamaño de la población fluctuante y como es el ciclo de vida del organismo.
- El modelo de equilibrio neutro-> la población se mantiene igual, implica un test donde la población encuentra esa distribución.
- El modelo de no equilibrio, la población fluctúa obteniendo diferentes distribuciones.
- Otro modelo es la selección constante, de la selección natural (irrealista).
- Otro donde la selección fluctúa logrando hacer la misma predicación que el modelo neutral.
- Lo correcto es encontrar el mejor modelo aunque se desvié del objetivo de rechazar la hipótesis nula.
- La probabilidad igualada no es una teoría 
- La teoría de un modelo particular de fuerzas faltantes no muestra que es el modelo, es el productor para otros modelos causales.

---
## No ecología nula
"El análisis de la "hipótesis nula"  de Connor y  Simberloff se caracteriza por una estructura oculta, ineficiencia, falta de sentido común, imprudencia y debilidad estadística, y en ultima instancia, por un escandaloso desprecio por su propio procedimiento" Diamond y Gilpin.

No existe una unica manera de permutar una matriz para encontrar un modelo nulo particular.
Métodos como procedimientos de asignación cuadrática estadísticamente no hacen lo que dicen hacer porque no existe una unica red nula.

---
## Hipótesis y modelos
La investigación requiere más que robots nulos
- Modelos causales generativos -> simular datos del modelo
- Modelos estadísticos justificados por modelos generativos y preguntas (estimaciones)
- Una forma efectiva de hacer estimaciones
- Después de que funciona con modelos simulados se introduce con los datos reales.
- Modelo quístico -> Relación entre dos variables particulares y sabemos que hay más variables.
---
Para elegir uno necesita un DAG, más que un modelo generativo que especifique las relaciones de forma entre las variables, causa problemas cuando agregas control de variables.

### Data finita, infinitos problemas
DAG no es suficiente.
Necesita modelos generativos/ depurar la ineficiencia
Necesita estrategia para derivar estimados e incertidumbre.
El enfoque mas sencillo: Análisis data Bayesiano

---
## Bayes es practico, no filosófico 
Análisis simples: pequeñas diferencias, añade desorden 
Análisis realista: diferencia
Error de medida, data perdida variables latentes, regularización.
Los modelos son generativos -> simula data como modelo causal
La acción es en machine learning, diferentes batallas.

---
## Búho
Solo te dicen como iniciar y el resto lo haces tu mismo.
El resto de pasos va muy rápido, para ir lento es mejor darse cuenta en que parte tienen problemas, más tiempo, pero efectivo.
Flujo de trabajo -> simulación generativa por pasos
El análisis de datos científicos es un software amateur de ingeniería 
Scripting es mejor -> comentar apropiadamente
Tres modos:
1. Entiende que estas haciendo ->workflow donde se mantiene
2. Documentar tu error, reduce el error
3. Flujo de trabajo científico respectivo

Pasos de Búho Bayes
1. Estimación teórica
2. Modelo (s) científico (s)
3. Usar 1 &2 para crear modelo estadístico
4. Simular de 2 para validar 3 produce 1
5. Analiza data real
