# Inteligencia estratégica de negocio: IA generativa en educación (Scopus 2020–2026)

**Por: Darío Castro Uribe y Ludys Cardozo Barragan**

---

## 1) Problemática de negocio

Las instituciones educativas necesitan decidir cómo adoptar IA generativa (ChatGPT/LLMs) maximizando beneficios (tutoría, retroalimentación, diseño instruccional) y minimizando riesgos (integridad académica, privacidad, sesgos).

**Pregunta de negocio:**  
¿Cómo evoluciona la evidencia científica (temas + sentimiento) sobre IA generativa en educación y cuál es la tendencia de crecimiento de publicaciones para orientar decisiones en los próximos 24 meses?

---

## 2) Datos

- **Fuente:** Scopus (export CSV)
- **Periodo:** 2020–2026
- **Idioma:** español
- **Registros trabajados en Colab:** 316 (tras limpieza y disponibilidad de abstract)

---

## 3) Metodología (flujo)

1. Carga y limpieza del CSV (`year`, `abstract`)
2. Bibliometría (Bibliometrix/Biblioshiny): mapa temático, red de co-ocurrencia, fuentes relevantes y producción anual
3. NLP (BERT): sentimiento por abstract y promedio anual
4. Estadística (PDF) + ML: modelado de tendencia y predicción
5. Dashboard/Reporte: exportables en PNG/PDF y texto interpretativo (LLM)
6. Estrategias de negocio + KPIs

---

## 4) Estructura del repositorio

- `notebooks/`: notebook reproducible (.ipynb)
- `outputs/`: gráficos exportados (PNG/PDF)

---

## 5) Cómo ejecutar (Colab)

1. Abrir el notebook en `notebooks/`
2. Montar Drive
3. Ajustar la variable `CSV_META` con la ruta del CSV
4. Ejecutar las celdas en orden

---

## 6) Resultados y visualizaciones

### Producción científica anual

![Producción anual](outputs/annual_production.png)

**Interpretación:**  
Se evidencia crecimiento sostenido de publicaciones sobre IA generativa en educación entre 2020 y 2026, indicando expansión del interés científico y relevancia estratégica del tema.

---

### Red de co-ocurrencia

![Coocurrencia](outputs/cooccurrence_network.png)

**Interpretación:**  
Las palabras clave muestran relaciones temáticas relevantes y conexiones entre conceptos asociados a inteligencia artificial, aprendizaje y educación.

---

### Mapa temático

![Mapa temático](outputs/thematic_map.png)

**Interpretación:**  
Se identifican líneas temáticas emergentes y consolidadas, permitiendo reconocer tendencias y áreas de investigación con mayor desarrollo.

---

### Fuentes relevantes

![Fuentes](outputs/most_relevant_sources.png)

**Interpretación:**  
Se destacan revistas y fuentes académicas líderes en la producción científica relacionada con IA generativa y educación.

---

### Sentimiento NLP

![Sentimiento](outputs/sentiment_over_time.png)

**Interpretación:**  
Predomina sentimiento positivo en los abstracts analizados, sugiriendo percepción favorable frente al uso de IA generativa en contextos educativos.

---

## 7) Evidencias (outputs)

Los gráficos del análisis se encuentran en la carpeta `outputs/` en formato PNG y PDF, permitiendo reproducibilidad y verificación de los resultados obtenidos.

---

## 8) KPIs estratégicos

Los indicadores clave de rendimiento (KPIs) permiten monitorear la evolución científica y apoyar decisiones estratégicas sobre adopción de IA generativa en educación.

| KPI | Indicador | Interpretación estratégica |
|---|---|---|
| Crecimiento de publicaciones | Variación anual de publicaciones | Mide expansión del campo científico |
| Sentimiento positivo | Proporción de abstracts positivos | Evalúa percepción académica favorable |
| Intensidad temática | Frecuencia de palabras clave | Identifica temas dominantes y emergentes |
| Precisión del modelo predictivo | Error o ajuste del modelo ML | Evalúa confiabilidad de las predicciones |

**Aplicación estratégica:**  
Estos KPIs permiten monitorear la madurez del tema, anticipar cambios y orientar decisiones institucionales relacionadas con innovación educativa y adopción de IA generativa.

---

## 9) Limitaciones del estudio

Aunque el análisis proporciona evidencia relevante para la inteligencia estratégica, se identifican algunas limitaciones metodológicas:

- La base de datos utilizada corresponde exclusivamente a Scopus.
- El análisis de sentimiento se realizó sobre abstracts y no sobre textos completos.
- El modelo predictivo depende del comportamiento histórico observado y puede verse afectado por cambios disruptivos futuros.
- La literatura científica en otros idiomas o bases de datos podría estar subrepresentada.

Estas limitaciones deben considerarse al interpretar los resultados y formular decisiones estratégicas.

---

## 10) Conclusiones

1. La producción científica sobre IA generativa en educación presenta crecimiento sostenido durante el periodo 2020–2026, evidenciando consolidación y expansión temática.

2. El análisis bibliométrico identifica relaciones significativas entre inteligencia artificial, aprendizaje y transformación educativa, mostrando convergencia temática relevante.

3. El análisis de sentimiento evidencia predominancia de percepciones positivas respecto al uso de IA generativa en educación, aunque persisten preocupaciones relacionadas con ética e integridad académica.

4. El uso combinado de bibliometría, NLP y Machine Learning fortalece la inteligencia estratégica al integrar análisis descriptivo, interpretativo y predictivo.

---

## 11) Implicaciones para la toma de decisiones

Los hallazgos del estudio aportan evidencia para orientar decisiones estratégicas en instituciones educativas.

| Hallazgo | Decisión sugerida |
|---|---|
| Crecimiento sostenido de publicaciones | Fortalecer procesos de innovación y vigilancia tecnológica |
| Sentimiento mayoritariamente positivo | Diseñar pilotos institucionales de IA generativa |
| Temas emergentes identificados | Impulsar capacitación docente y actualización curricular |
| Riesgos éticos presentes | Formular políticas de uso responsable y gobernanza digital |

**Interpretación estratégica:**  
Los resultados sugieren que las instituciones educativas deberían avanzar hacia modelos graduales de adopción de IA generativa, acompañados de formación, protocolos éticos y evaluación continua de impacto.
