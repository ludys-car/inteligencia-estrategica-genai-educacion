# Inteligencia estratégica de negocio: IA generativa en educación (Scopus 2020–2026)
Por: José Darío Castro Uribe y Ludys Cardozo Barragán

## 1) Caso / problemática de negocio
Las instituciones educativas (universidades/colegios y edtech) deben decidir cómo adoptar IA generativa (ChatGPT/LLMs) maximizando beneficios (tutoría, retroalimentación, diseño instruccional) y minimizando riesgos (integridad académica, privacidad, sesgos).

**Pregunta de negocio:** ¿Cómo evoluciona la evidencia científica (temas + sentimiento) sobre IA generativa en educación y cuál es la tendencia de crecimiento de publicaciones para orientar decisiones de adopción responsable en los próximos 24 meses?

---

## 2) Datos
- Fuente: Scopus (export CSV).
- Filtros aplicados: 2020–2026, idioma español, artículos (ar) y conferencia (cp).
- Variable textual principal: `Abstract` (para NLP).
- Variable temporal: `Year` (para tendencia y predicción).

> Nota: En Biblioshiny se importaron 344 registros. Para análisis en Colab se trabajó con 316 registros tras limpieza (abstract no vacío) y filtro 2020–2026.

---

## 3) Metodología (flujo analítico integrado)
1) **Carga y limpieza del CSV** (normalización de columnas, filtro temporal, depuración de abstracts).
2) **Bibliometría (Bibliometrix/Biblioshiny)**: mapa temático, red de co-ocurrencia, fuentes relevantes, producción anual.
3) **NLP (BERT)**: sentimiento por abstract y agregación anual.
4) **Estadística (PDF)**: densidad del conteo anual de publicaciones (KDE/Normal ajustada).
5) **ML (predicción)**: modelo de tendencia para pronosticar publicaciones futuras.
6) **Dashboard/Reporte**: exportables en PNG/PDF + interpretación estratégica (LLM).
7) **Estrategias y KPIs**: diseño de acciones y métricas para toma de decisiones.

---

## 4) Evidencias visuales (outputs)
### Bibliometría (Bibliometrix/Biblioshiny)
- Mapa temático (Thematic Map):
  - PNG: `outputs/thematic_map.png`
  - PDF: `outputs/thematic_map.pdf`

![Mapa temático](outputs/thematic_map.png)

- Red de co-ocurrencia:
  - PNG: `outputs/cooccurrence_network.png`
  - PDF: `outputs/cooccurrence_network.pdf`

![Red de co-ocurrencia](outputs/cooccurrence_network.png)

- Fuentes más relevantes:
  - PNG: `outputs/most_relevant_sources.png`
  - PDF: `outputs/most_relevant_sources.pdf`

![Fuentes más relevantes](outputs/most_relevant_sources.png)

- Producción anual:
  - PNG: `outputs/annual_production.png`
  - PDF: `outputs/annual_production.pdf`

![Producción anual](outputs/annual_production.png)

### Estadística + ML (tendencia)
- PDF (densidad): `outputs/pdf_publications_density.pdf`
- PDF (predicción ML): `outputs/ml_forecast_publications.pdf`

---

## 5) Interpretación para toma de decisiones (aporte empresarial)
**Hallazgo 1 — Temas dominantes:** El núcleo del campo se organiza alrededor de educación + IA/ChatGPT, lo que indica alta relevancia y demanda de lineamientos pedagógicos y de gobernanza.  
**Decisión sugerida:** avanzar con adopción controlada, priorizando rediseño de evaluación y formación docente.

**Hallazgo 2 — Líneas especializadas:** ética/integridad académica, pensamiento crítico/creatividad y formación docente aparecen como líneas clave que condicionan la adopción.  
**Decisión sugerida:** establecer política institucional y protocolos (uso permitido/no permitido) antes de escalar.

**Hallazgo 3 — Sentimiento y tendencia:** el sentimiento anual y el crecimiento de publicaciones funcionan como señal de madurez del tema.  
**Decisión sugerida:** pilotos con métricas en el corto plazo y escalamiento progresivo si la tendencia se mantiene al alza y el discurso se estabiliza.

---

## 6) Estrategias de negocio (a 24 meses)
1) **Gobernanza y uso responsable**
   - Política de uso, privacidad, integridad académica, verificación y transparencia.
2) **Pilotos pedagógicos de alto valor**
   - Casos de uso priorizados: feedback, tutoría, apoyo a escritura, diseño instruccional.
3) **Capacitación y rediseño de evaluación**
   - Alfabetización en IA (docentes/estudiantes) + evaluación auténtica.

---

## 7) KPIs (indicadores clave)
### Estrategia 1 — Gobernanza
- % de programas/asignaturas con política de uso publicada.
- # incidentes de integridad académica asociados a IA por semestre.
- % cumplimiento de requisitos de privacidad/gobernanza (checklist institucional).

### Estrategia 2 — Pilotos de alto valor
- Reducción del tiempo promedio de retroalimentación (horas/días).
- % estudiantes que reportan mejora en calidad del feedback (encuesta).
- Mejora en desempeño en evaluaciones auténticas (rúbrica).

### Estrategia 3 — Capacitación + evaluación
- % docentes certificados en alfabetización en IA.
- % estudiantes que completan módulo de uso responsable.
- # asignaturas con evaluación rediseñada (autenticidad/proceso).

---

## 8) Limitaciones metodológicas
- Cobertura limitada a **Scopus**, idioma español y periodo 2020–2026 (sesgo de cobertura).
- El análisis bibliométrico depende de la calidad de metadatos (keywords/abstracts).
- El análisis de sentimiento (BERT) trabaja sobre abstracts: no representa todo el contenido del artículo.
- La predicción ML usa pocos puntos temporales (años), por lo que la incertidumbre es alta (se recomienda actualizar con nuevos años y comparar modelos).

---

## 9) Conclusiones
- IA generativa en educación es un campo de alta centralidad temática, con discusión creciente sobre ética, evaluación e integridad académica.
- La evidencia respalda adopción **gradual y gobernada**, con pilotos medibles y capacitación como habilitadores.
- La combinación bibliometría + NLP + ML mejora la lectura estratégica al conectar “qué se investiga”, “cómo se discute” y “hacia dónde crece” el campo.

---

## 10) Cómo ejecutar (Colab)
1. Abrir el notebook en `notebooks/`.
2. Montar Drive.
3. Ajustar la variable `CSV_META` con la ruta del CSV en Drive.
4. Ejecutar las celdas en orden (Runtime → Run all).

---

## 11) Estructura del repositorio
- `notebooks/`: notebook reproducible (.ipynb)
- `outputs/`: gráficos y PDFs (evidencias)
