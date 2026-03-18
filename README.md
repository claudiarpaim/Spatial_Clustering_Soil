# Clusterização Espacial de Solos com Machine Learning

## Descrição do Projeto

Este projeto aplica técnicas de aprendizado não supervisionado para identificar padrões espaciais em propriedades físico-químicas do solo.

A partir de dados geoespaciais do SoilGrids, foi construída uma base de dados estruturada contendo variáveis como pH, carbono orgânico, nitrogênio, textura e densidade do solo.

O objetivo é responder à seguinte pergunta:

> É possível identificar zonas homogêneas de solo utilizando técnicas de Machine Learning?

---

## Objetivos

- Construir um dataset a partir de rasters geoespaciais  
- Analisar a estrutura multivariada dos dados  
- Reduzir dimensionalidade com PCA  
- Identificar padrões com clusterização (K-Means)  
- Interpretar os clusters no contexto ambiental  

---

## Metodologia

O projeto foi dividido em três etapas principais:

### 1. Construção do Dataset
- Leitura de rasters (GeoTIFF)
- Empilhamento das variáveis
- Conversão para estrutura tabular
- Tratamento de valores inválidos

### 2. Análise Exploratória e PCA
- Análise de correlação
- Padronização dos dados
- Redução de dimensionalidade (PCA)
- Identificação de gradientes estruturais

### 3. Clusterização
- Aplicação do K-Means
- Definição do número de clusters
- Análise dos perfis de solo
- Visualização espacial dos agrupamentos

---

## Principais Resultados

- Identificação de padrões espaciais consistentes no solo  
- Evidência de dois gradientes dominantes: químico e textural  
- Segmentação do solo em grupos com características distintas  
- Coerência espacial dos clusters  

---

## Aplicações

- Planejamento agrícola  
- Manejo do solo  
- Zoneamento ambiental  
- Apoio à tomada de decisão  

---

## Tecnologias Utilizadas

- Python
- NumPy
- Pandas
- Rasterio
- Scikit-learn
- Matplotlib / Seaborn

---

## 📁 Estrutura do Projeto

soil-clustering-ml/
│
├── data/
│   ├── raw/              # rasters originais (ou link se forem grandes)
│   └── processed/        # dataset final
│
├── notebooks/
│   01_dataset_construction.ipynb
│   02_exploratory_analysis_pca.ipynb
│   03_clustering_spatial_patterns.ipynb
│
├── images/               # salvar gráficos importantes (opcional)
│
├── src/                  # (opcional futuramente)
│
├── README.md             ⭐ (mais importante)
├── requirements.txt
└── .gitignore

