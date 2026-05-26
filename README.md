# Inteligencia estratégica de negocio: IA generativa en educación (Scopus 2020–2026)
 Por: Darío Castro Uribe, Ludys Cardozo Barragán

## 1) Problemática de negocio
Las instituciones educativas necesitan decidir cómo adoptar IA generativa (ChatGPT/LLMs) maximizando beneficios (tutoría, retroalimentación, diseño instruccional) y minimizando riesgos (integridad académica, privacidad, sesgos).

**Pregunta de negocio:** ¿Cómo evoluciona la evidencia científica (temas + sentimiento) sobre IA generativa en educación y cuál es la tendencia de crecimiento de publicaciones para orientar decisiones en los próximos 24 meses?

## 2) Datos
- Fuente: Scopus (export CSV)
- Periodo: 2020–2026
- Idioma: español
- Registros trabajados en Colab: 316 (tras limpieza y disponibilidad de abstract)

## 3) Metodología (flujo)
1. Carga y limpieza del CSV (year, abstract)
2. Bibliometría (Bibliometrix/Biblioshiny): mapa temático, red de co-ocurrencia, fuentes relevantes, producción anual
3. NLP (BERT): sentimiento por abstract y promedio anual
4. Estadística (PDF) + ML: modelado de tendencia y predicción
5. Dashboard/Reporte: exportables en PNG/PDF y texto interpretativo (LLM)
6. Estrategias de negocio + KPIs

## 4) Estructura del repositorio
- `notebooks/`: notebook reproducible (.ipynb)
- `outputs/`: gráficos exportados (PNG/PDF)

## 5) Cómo ejecutar (Colab)
1. Abrir el notebook en `notebooks/`
2. Montar Drive
3. Ajustar la variable `CSV_META` con la ruta del CSV
4. Ejecutar las celdas en orden

## 6) Evidencias (outputs)
Los gráficos del análisis se encuentran en la carpeta `outputs/` (PNG/PDF).
