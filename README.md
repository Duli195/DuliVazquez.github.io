# DuliVazquez.github.io

# Proyecto KPIs y Operaciones Logísticas
Este proyecto tiene como objetivo diseñar y analizar una base de datos relacional para operaciones logísticas, utilizando SQLite y Python sin necesidad de archivos externos.  
El sistema simula el funcionamiento de una empresa de distribución que gestiona productos, almacenes, inventarios, órdenes, clientes y entregas, permitiendo calcular indicadores clave de desempeño (KPIs) y realizar consultas operativas en tiempo real.

---
## Modelo de datos
El modelo integra siete tablas principales:  
`productos`, `almacenes`, `inventario_actual`, `movimientos_almacen`, `clientes`, `ordenes`, y `entregas`.  
A partir de ellas, se ejecutan consultas SQL que miden el rendimiento de las operaciones y ayudan a detectar áreas de mejora en la cadena de suministro.

---
## Principales KPIs generados
- **On-Time Delivery Rate:** mide entregas puntuales.  
- **In-Full Rate:** mide pedidos entregados en su totalidad.  
- **OTIF (On Time In Full):** combina puntualidad y completitud.  
- **Lead Time Promedio:** calcula el tiempo medio entre orden y entrega.  
- **Rotación de productos:** muestra los productos con mayor movimiento.  
- **Inventario valorizado:** estima el valor total del stock por almacén.  
Además, se desarrollaron consultas adicionales para detectar backorders, alertas de inventario bajo, puntualidad y retrasos por transportista, y fill rate promedio por producto.  
Estos indicadores permiten tomar decisiones más informadas sobre eficiencia operativa, control de inventarios y desempeño logístico.

---
##Conclusiones
El proyecto demuestra que una **base de datos bien estructurada** puede convertirse en una herramienta esencial para **analizar el rendimiento logístico** y detectar oportunidades de mejora.  
La integración de **Python y SQL** permite automatizar cálculos de KPIs y generar reportes actualizables de manera eficiente, contribuyendo a la **toma de decisiones estratégicas**.  
Los resultados obtenidos evidencian la importancia del **seguimiento de entregas**, la **gestión de inventarios** y la **precisión documental** para mantener altos niveles de servicio al cliente.  
En conjunto, este trabajo reafirma el valor del **análisis de datos en la logística moderna**, al convertir la información operativa en **conocimiento útil para la planificación, control y mejora continua**.




# Proyecto de Recuperación de Oro — Análisis Predictivo
## Descripción general
Este proyecto se enfoca en el **análisis y predicción de la eficiencia de recuperación de oro** en un proceso industrial de flotación y purificación.  
El objetivo principal fue desarrollar un modelo predictivo que permitiera estimar el nivel de recuperación del metal precioso a partir de datos históricos del proceso, optimizando así la producción y mejorando la toma de decisiones operativas.
El análisis incluyó la **validación de fórmulas metalúrgicas**, la **limpieza de datos**, la **detección de anomalías** y la construcción de modelos de aprendizaje automático para estimar la recuperación en distintas etapas del proceso.  
A través de un enfoque de evaluación y comparación de modelos, se identificó la alternativa con mejor desempeño, destacando la importancia de la calidad de los datos y la coherencia física en el modelado predictivo.

---
## Resultados generales
Durante la validación, se comprobó la coherencia entre los valores reales y los calculados de recuperación, con un **error promedio aceptable**, lo que confirmó la consistencia general de los datos.  
Posteriormente, los modelos predictivos desarrollados fueron evaluados con la métrica **sMAPE (Symmetric Mean Absolute Percentage Error)**, dando como resultado un desempeño satisfactorio, especialmente en la predicción de la etapa final del proceso.
El modelo mostró mayor precisión en la **recuperación final**, la etapa más relevante para la producción y rentabilidad, mientras que la **recuperación rougher** presentó mayor variabilidad, indicando margen de mejora en fases tempranas del proceso.

---
## Conclusiones
- El proyecto demuestra la **viabilidad del uso de modelos predictivos** para estimar la eficiencia de recuperación del oro y optimizar los procesos industriales.  
- La **calidad y consistencia de los datos** son factores determinantes para lograr predicciones precisas y confiables.  
- La **validación física y eliminación de anomalías** antes del modelado fue clave para obtener resultados coherentes.  
- Aunque los modelos ofrecen un buen desempeño general, se identifican oportunidades para mejorar la precisión en las primeras etapas del proceso mediante ajustes de parámetros o el uso de modelos más avanzados.  
- En conjunto, este trabajo evidencia el potencial del análisis de datos para **incrementar la eficiencia, reducir pérdidas y apoyar la toma de decisiones** en entornos productivos.




# Análisis del Mercado de Videojuegos — Tendencias, Ventas y Preferencias Regionales
## Descripción general
Este proyecto tiene como objetivo **analizar el comportamiento del mercado global de videojuegos**, explorando cómo las ventas, géneros, plataformas y calificaciones han evolucionado a lo largo del tiempo.  
A partir del conjunto de datos `games.csv`, se realizó un proceso de **preparación, limpieza y análisis exploratorio** para identificar patrones en los lanzamientos, las preferencias de los jugadores y las diferencias entre regiones.  
El estudio abarca desde la detección de valores ausentes hasta pruebas estadísticas que comparan las calificaciones de los usuarios entre plataformas y géneros.
Durante el análisis se desarrollaron visualizaciones descriptivas que muestran:
- La evolución del número de lanzamientos por año.  
- Las plataformas con mayores ventas globales y regionales.  
- La distribución de ventas por género y región.  
- La relación entre las reseñas de críticos y usuarios con las ventas.  
- Las diferencias significativas en calificaciones entre plataformas y tipos de juegos.
  
---
## Conclusiones
### Preparación y limpieza de datos
- Se revisaron y transformaron las columnas para corregir errores de formato, convertir tipos de datos y tratar valores ausentes.  
- Se reemplazaron los valores `'tbd'` de la columna `user_score` por `NaN` para evitar sesgos en el análisis.
   
---
### Análisis general
- El número de lanzamientos alcanzó su **pico entre 2008 y 2011**, seguido por una reducción en años posteriores.  
- Las **plataformas históricamente más exitosas** fueron **PS2**, **X360** y **Wii**, mientras que **PS4** y **3DS** dominaron los últimos años del análisis.  
- Los **géneros de Acción, Deporte y Shooter** concentraron la mayoría de las ventas globales.  
- Se observó una **correlación positiva entre las críticas de expertos y las ventas**, especialmente en plataformas como PS4, mientras que la influencia de las calificaciones de usuarios fue más débil.
  
---
### Preferencias regionales
- **Norteamérica y Europa** mostraron preferencia por consolas de sobremesa como **X360** y **PS3**.  
- **Japón** destacó por su preferencia hacia **plataformas portátiles** como **3DS** y **DS**, y por su afinidad con los juegos de **Rol (RPG)**.  
- Las **clasificaciones ESRB** influyeron más en los mercados de **NA y EU** que en Japón.
  
---
### Resultados de las pruebas de hipótesis
- **H₁:** Se detectó una **diferencia significativa** entre las calificaciones promedio de usuarios en **Xbox One y PC**, lo que sugiere distintos perfiles de usuario por plataforma.  
- **H₂:** **No se encontró diferencia significativa** entre las calificaciones de los géneros **Acción y Deportes**, lo que indica una percepción similar entre jugadores en esos segmentos.
  
---
### Recomendaciones
- Enfocar las campañas de marketing de **juegos de acción y disparos** en los mercados de **Norteamérica y Europa**, especialmente en **PS4** y **XOne**.  
- En **Japón**, priorizar la promoción de **juegos de rol (RPG)** en consolas portátiles.  
- Considerar la **influencia de las reseñas de críticos** como un indicador clave de ventas futuras.  




# Análisis de Vehículos en Venta en Estados Unidos
## Descripción general
Este proyecto tiene como propósito **analizar las características y tendencias de los vehículos en venta en Estados Unidos**, utilizando datos provenientes de anuncios reales.  
A través de la exploración visual de los datos, se busca comprender cómo factores como el **kilometraje (odómetro)** y el **precio de venta** se relacionan entre sí, con el fin de identificar patrones relevantes en el mercado automotriz de segunda mano.  
El análisis se basa en la creación de visualizaciones dinámicas que permiten observar:
- La **distribución del kilometraje** de los vehículos disponibles.  
- La **relación entre el odómetro y el precio**, mostrando cómo el uso y la antigüedad influyen en el valor de mercado.  
Estas visualizaciones permiten al usuario explorar la información de forma interactiva, facilitando la detección de tendencias y comportamientos generales dentro del mercado automotriz.

---
## Conclusiones
- La mayoría de los vehículos en venta presentan **niveles moderados de kilometraje**, lo cual sugiere una alta rotación de autos usados en condiciones intermedias de uso.  
- Se observa una **relación inversa entre el kilometraje y el precio**: los autos con mayor recorrido tienden a tener un valor de venta más bajo, lo que confirma una tendencia esperada en el mercado.  
- Existen **casos atípicos** (vehículos con alto kilometraje pero precios elevados) que podrían corresponder a autos de lujo o a modelos con mantenimiento excepcional.  
- El análisis visual facilita la comprensión de los **factores que más influyen en el precio**, ofreciendo una base para decisiones de compra, venta o tasación de vehículos usados.  
En conjunto, el proyecto demuestra cómo el análisis exploratorio de datos permite **detectar patrones significativos y apoyar decisiones informadas** dentro del mercado de automóviles de segunda mano.
