# BETO Legal RAG Engine

[![Status](https://img.shields.io/badge/status-in_development-yellow.svg)]()
[![Python](https://img.shields.io/badge/python-3.10+-blue.svg)]()
--- 
Este repositorio alberga el **motor de RAG (Retrieval-Augmented Generation)** diseñado específicamente para potenciar **BETO Legal México**. 

El objetivo es mejorar la efectividad de las respuestas de BETO mediante la recuperación contextual precisa de documentos jurídicos mexicanos, reduciendo alucinaciones y aumentando la relevancia legal de las salidas.

## 🚀 Estado del Proyecto
Actualmente en fase de **desarrollo activo**. Se está trabajando en la optimización de la búsqueda semántica y la integración del pipeline de ingestión documental.

## 🛠 Arquitectura Técnica
*   **Base de Modelos:** Basado en arquitectura BERT/RigoBERTa.
*   **Pipeline RAG:**
    *   **Ingestión:** Procesamiento de documentos judiciales obtenidos vía scrapers (SCJN).
    *   **Indexación:** Implementación de bases de datos vectoriales para almacenamiento de embeddings.
    *   **Recuperación:** Estrategias de *hybrid search* (búsqueda semántica + búsqueda por palabras clave/bm25).
*   **Framework:** Python 3.10+.

## 📋 Roadmap
- [ ] Refinamiento del chunking de documentos legales para preservar el contexto de las leyes.
- [ ] Optimización de la latencia en la recuperación (Retrieval).
- [ ] Evaluación del pipeline RAG mediante métricas de fidelidad y relevancia.
- [ ] Integración con el modelo principal de BETO Legal.

## 📦 Estructura del Repo
```text
├── data/           # Documentos legales procesados
├── src/            # Lógica del motor RAG
├── notebooks/      # Pruebas de concepto y experimentos con embeddings
└── tests/          # Suite de validación de efectividad

```

## 💻 Desarrollo Local

```bash
# Clonar repo
git clone [https://github.com/brams153/BETO-Legal-RAG-Engine]

# Instalación de dependencias (se recomienda usar uv)
uv sync

```

## 🤝 Contribuciones

Proyecto personal en desarrollo. Si tienes sugerencias sobre la estrategia de recuperación o el manejo de embeddings legales, abre un *issue*.

---

*Desarrollado como parte del ecosistema de BETO Legal México.*
