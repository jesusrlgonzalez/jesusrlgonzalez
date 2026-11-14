# Jesús R. L. González

**Ciencia de datos para calidad y manufactura.** Licenciado en Ingeniería Industrial y Administración, con formación dual alemana (IHK Regensburg, en planta con ISO 9001) y curso de Auditor Líder ISO 9001:2015 certificado por CQI-IRCA, aprobado. Traduzco scrap, alertas de falla y defectos a decisiones con costo, y digo cuándo los datos **no** alcanzan para desplegar un modelo.

📍 Tlaxcala–Puebla, México · 🗣️ Español nativo · Alemán profesional · Inglés A2 en formación
🔗 [LinkedIn](https://www.linkedin.com/in/jesus-r-l-gonzalez) · [Portafolio con demos](https://huggingface.co/spaces/JesusRLGonzalez/jesus-rl-gonzalez)

## Casos públicos

Cada caso declara si sus datos son reales, simulados o sintéticos. Los resultados con datos simulados o sintéticos demuestran el método, no impacto en un cliente.

| Decisión | Datos | Resultado | Validación | Demo | Código |
|---|---|---|---|---|---|
| ¿Qué alertas de la flota merecen ir a taller? | Reales · Scania APS (reto IDA 2016) | De 187,500 a 11,540 **unidades de costo del reto** (−94 %), 359 de 375 fallas detectadas. No es un ahorro medido en una empresa | Conjunto de prueba oficial, evaluado una sola vez | [Demo](https://jesusrlgonzalez.github.io/aps-failure-intelligence/) | [Repo](https://github.com/jesusrlgonzalez/aps-failure-intelligence) |
| ¿Vale la pena desplegar un modelo de calidad? | Reales · UCI SECOM, 1,567 lotes | Ahorro no distinguible de cero (IC 95 % incluye el cero) → **no desplegar** | Temporal: últimos 313 lotes, evaluados una vez | [Demo](https://jesusrlgonzalez.github.io/predictive-quality-mlops/) | [Repo](https://github.com/jesusrlgonzalez/predictive-quality-mlops) |
| ¿Adónde se va el costo de la no calidad? | Sintéticos · planta de autopartes | Palancas **estimadas** en 1.23 M MXN al año (14.5 % del COPQ) | Temporal: entrena ene–sep, evalúa oct–dic | [Demo](https://jesusrlgonzalez.github.io/scrap-copq-analytics/) | [Repo](https://github.com/jesusrlgonzalez/scrap-copq-analytics) |
| ¿Qué equipos intervengo esta semana? | Simulados · NASA C-MAPSS FD001 | −40 % de costo frente al reemplazo por edad, en backtest | Validación cruzada agrupada por motor y conjunto de prueba oficial | [Demo](https://jesusrlgonzalez.github.io/predictive-maintenance-survival-cmapss/) | [Repo](https://github.com/jesusrlgonzalez/predictive-maintenance-survival-cmapss) |
| ¿Qué defectos de placa debe revisar una persona? | Reales · 1,941 placas de acero (UCI) | Macro-F1 0.815 en holdout | Estratificada: holdout de 389 placas, evaluado una vez (los datos no tienen fechas) | [Demo](https://jesusrlgonzalez.github.io/steel-plates-quality-mlops/) | [Repo](https://github.com/jesusrlgonzalez/steel-plates-quality-mlops) |
| ¿Cuánto dejar en cada tienda de la ruta? | Sintéticos · tiendas de abarrotes | Error de pronóstico (WAPE) de 31.7 % a 22.1 % | Temporal: entrena ene 2024–jun 2025, evalúa jul–dic 2025 | [Demo](https://jesusrlgonzalez.github.io/predix/) | [Repo](https://github.com/jesusrlgonzalez/predix) |

**Límites de despliegue.** Ningún modelo opera hoy en una planta. Las demos corren con datos públicos o de ejemplo, y las que aceptan tu archivo lo procesan en tu navegador. Los costos son supuestos declarados en cada repositorio. Pasar a producción requeriría datos propios del proceso, un piloto en paralelo y monitoreo.

## Cómo trabajo

Línea base primero · validación sin fuga de información (temporal cuando los datos tienen fechas; estratificada o agrupada cuando no las tienen) · umbral elegido por costo del error · intervalos de confianza en cada cifra que importa · límites declarados en cada README.

**Herramientas:** Python (pandas, scikit-learn, statsmodels) · SQL (PostgreSQL, DuckDB) · Power BI (DAX) · Streamlit · FastAPI · Docker · GitHub Actions · control estadístico de procesos · análisis de supervivencia.

## Conectemos

Me interesa conversar con ingenieros de procesos, calidad, mantenimiento y operaciones, y con equipos de datos en manufactura. Escríbeme por [LinkedIn](https://www.linkedin.com/in/jesus-r-l-gonzalez).
