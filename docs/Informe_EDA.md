Al realizar un análisis exploratorio de los datos, se pudo observar tanto en la estadística descriptiva como en los gráficos, que la **demanda de gas natural en Argentina está dominantemente impulsada por la estacionalidad climática y, específicamente, por la necesidad de calefacción en el sector residencial.**

De los datos se encontró:

* **Validación de la Demanda Climática (GDC)**  
  Se ven validadas las fuertes asimetrías y el papel central del GDC. La temperatura promedio tiene un rango amplio(es importante considerar que esa columna agrupa diferentes provincias, por lo cual es lógica la variación dada, justamente, la variación de amplitud térmica a lo largo de Argentina). Esta gran variabilidad impulsa la estacionalidad.  
    
* **Asimetría del GDC:**  
  Hay asimetría en el gdc, pues los dos primeros cuartiles son igual a 0 (Recordando además, que el segundo cuartil equivale a la mediana). Esta asimetría se **cuantifica** en el histograma donde se observa que al menos el **50% de los meses registrados no tienen necesidad de calefacción** (meses cálidos), lo que confirma la segmentación de la demanda. Por otro lado, la **media del gdc es de 45.45** no coincidiendo con la mediana por mucho, lo que es un signo evidente de la asimetría positiva generada por los picos de invierno.  
* **Consumo y Demanda**  
  El análisis de las variables de consumo confirma que la demanda de calefacción genera la mayor variabilidad y los picos más extremos.  
  * **Consumo Residencial Extremo:** El consumo promedio (mean) del sector **residencial es 811.64**, pero su **máximo es 1770.06** levemente más del doble.  
    El **desvío estándar (std) es 485.66**, en relación con la media, es muy extremo. Esto significa que el consumo residencial es la **variable más volátil** y sensible a los picos de frío.  
  * **Consumo 'Otros sectores':** A comparación del consumo residencial, el desvío estándar de **Otros sectores es 213.09** es mucho menor. Esto sugiere que el consumo de otros sectores se mantiene **más estable** y menos influenciado por las variaciones extremas de temperatura.  
      
  * **Producción vs. Total:** La media de producción de gas natural es de 3939.55, la cual es superior a la media de total (total suma el gas residencial y otros sectores), quien cuenta con una media de 3627.44, lo que sugiere que, en promedio, hay un excedente de producción destinado (para exportación, almacenamiento o pérdidas), pero esto se revierte durante los picos de demanda invernal (observado en el gráfico de barras).  
    

**Conclusiones**

 **El Clima y la Demanda**

* **Dominancia del Frío:** La **temperatura promedio** muestra una distribución bimodal, confirmando dos regímenes climáticos: cálido (verano) y frío (invierno), lo que explica la estacionalidad del consumo.  
* **Validación de la Métrica (GDC):** El **Grado Día de Calefacción (GDC)** es la variable clave. El gráfico **GDC vs. Temperatura** confirma su cálculo basado en la temperatura base igual  a 18°C.  
* **Fuerte Correlación:** Los *pair plots* indican una relación **fuerte y positiva** entre el **GDC** y el consumo de gas, lo que prueba que la necesidad de calefacción es el principal impulsor de la demanda.

**Patrones de Consumo y Distribución (Volatilidad)**

* **Pico Residencial:** El consumo del sector **residencial es el más volátil** y el principal motor del consumo total. Su **desviación estándar es la más alta**, y el valor máximo duplica su valor promedio, lo que apunta a **picos extremos de demanda** durante el invierno.  
* **Estabilidad en Otros Sectores:** El consumo de **Otros sectores** es relativamente más estable (menor desviación estándar), lo que sugiere que este consumo depende menos de las fluctuaciones climáticas extremas.  
* **Correlación de Proporciones:** La matriz de correlación muestra que el **consumo absoluto residencial** está correlacionado con su **participación porcentual**. Esto significa que cuando el consumo residencial aumenta, acapara una porción mucho mayor del suministro total, porque resulta que el consumo residencial **es tan dominante** que cuando la demanda total de gas sube, es porque el consumo residencial subió, y viceversa. Esta correlación tan fuerte  de \+0.99 valida la conclusión de que el sector residencial es el **principal impulsor** de los movimientos en el mercado del gas, tanto en términos de volumen como de distribución porcentual.

**Desafío Crítico del Suministro**

* **Brecha Invernal:** El gráfico de barras por estación muestra que el **Consumo total en Invierno** supera la **Producción destinada promedio**. Esto indica un déficit estructural en la estación fría, lo que requiere cubrir la demanda con importaciones o reservas.  
* **Impacto Geográfico:** El mapa de calor identifica a las provincias del Sur (ej., Tierra del Fuego, Santa Cruz) como **zonas de demanda constante** debido a sus bajas temperaturas crónicas, mientras que las provincias del centro/norte impulsan la variabilidad extrema en invierno.

