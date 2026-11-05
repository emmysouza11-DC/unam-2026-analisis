\# Análisis estadístico del examen de admisión UNAM 2026



Análisis distribucional de los puntajes del examen de admisión a licenciatura de la UNAM, comparando la primera aplicación en línea (2026) contra el comportamiento histórico (2021–2025) mediante divergencia de Kullback–Leibler y la prueba de Kolmogórov–Smirnov.



\## Contexto



En 2026 la UNAM aplicó por primera vez su examen de admisión en modalidad en línea. Los resultados mostraron un incremento inusual en los puntajes altos respecto a años anteriores, lo que generó controversia pública. Este proyecto examina, con datos abiertos, si ese cambio es compatible con la variación histórica del examen o constituye una desviación atípica.



\## Hallazgos principales



\- La divergencia KL de 2026 frente al histórico alcanzó \*\*0.339 nats\*\*, entre \*\*80 y 160 veces\*\* la variación normal año a año.

\- El estadístico D de Kolmogórov–Smirnov fue de \*\*0.293\*\*, frente a un rango histórico de 0.009–0.031.

\- El cambio no es un desplazamiento uniforme: la parte baja-media de la distribución se mantiene casi idéntica al histórico, mientras emerge una \*\*segunda población\*\* en los puntajes altos.

\- El patrón es consistente en las cuatro áreas de conocimiento, con mayor magnitud en las de alta demanda.



\## Reproducibilidad



El análisis está en el notebook `UNAM.ipynb`. Para reproducirlo:



1\. Descarga los datos del repositorio fuente (ver más abajo).

2\. Coloca el CSV en la ruta indicada al inicio del notebook.

3\. Ejecuta las celdas en orden.



Dependencias: `pandas`, `numpy`, `scipy`, `matplotlib`, `seaborn`.



\## Estructura del repositorio



\- `UNAM.ipynb` — notebook con el análisis completo.

\- `Análisis\_puntajes\_atípicos\_UNAM\_.tex` / `.pdf` — documento con la metodología y resultados.

\- `figuras/` — gráficos generados.



\## Fuente de datos



Los datos provienen del repositorio comunitario: [agn3si/ResultadosUNAM---data](https://github.com/agn3si/ResultadosUNAM---data), obtenidos por web-scraping de las páginas públicas de resultados de la DGAE-UNAM. Este proyecto no rehospeda los datos; enlaza a la fuente original.



\## Autor



Emmanuel Ramírez Souza — [LinkedIn](https://www.linkedin.com/in/emmanuel-souza-ab9259341/) · Proyecto independiente, sin afiliación con la UNAM.



\## Limitaciones



El análisis cuantifica la anomalía distribucional pero no identifica su causa. La inferencia hacia un factor externo se apoya en la forma del cambio, no en una prueba de mecanismo. No incluye los resultados del examen presencial de control (no disponibles en datos abiertos).

