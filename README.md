# 🧪 Análise da Qualidade do Ar nos EUA (2024) com Docker e Python

Este projeto realiza uma análise exploratória de dados sobre o **Air Quality Index (AQI)** nos Estados Unidos em 2024, utilizando **Python** e **Jupyter Notebook** dentro de um ambiente totalmente containerizado com **Docker**.

---

## 📌 Objetivos

- Tratar e preencher valores ausentes nos conjuntos de dados AQI.
- Gerar estatísticas descritivas e visualizações dos dados por estado, período e tipo de poluente.
- Demonstrar como empacotar um projeto de ciência de dados em um container Docker com reprodutibilidade garantida.

---

## 🐳 Executando com Docker

### Pré-requisitos

- Docker instalado ([guia de instalação](https://docs.docker.com/get-docker/))

### Instruções

1. Clone este repositório:
```bash
git clone https://github.com/carlos95soares/Docker-Air-Quality
cd seu-repositorio
```

2. Execute o container:
```bash
docker-compose up
```

3. Acesse o JupyterLab:
```
http://localhost:8888
```

4. Token de acesso:
```
Projeto
```

---

## 📂 Conteúdo da Imagem Docker

A imagem Docker já vem com os seguintes itens:

- Quatro arquivos `.csv` com dados de qualidade do ar (AQI)
- Dois notebooks Jupyter:
  - `Air Quality Index 2024.ipynb` (script completo de análise)
  - `Documentação Trabalho TDA.ipynb` (explicação e instruções)
- Bibliotecas Python pré-instaladas:  
  `pandas`, `scikit-learn`, `matplotlib`, `seaborn`, `plotly`, `kaleido`

---

## 🔬 Etapas da Análise

O notebook realiza as seguintes ações:

- Leitura e tratamento de dados de 4 arquivos diferentes (df44201, df42101, df42401, df42602)
- Preenchimento de valores ausentes de AQI com a média baseada em chaves específicas (state, county, site, parâmetro, POC)
- Remoção de registros inconsistentes ou incompletos
- Conversão de datas e extração de informações mensais
- Classificação dos valores de AQI em faixas qualitativas (Boa, Moderada, Não saudável etc.)
- Agrupamento e contagem por categoria
- Geração de gráficos com `matplotlib`, `seaborn` e `plotly`, incluindo:
  - Distribuição de AQI por estado
  - Evolução mensal da média de AQI por tipo de poluente
  - Mapas interativos por estado e gás
  - Ranking dos 20 locais com maior média de AQI

---

## 📊 Exemplos de Visualizações

- 📈 Evolução mensal da qualidade do ar por gás
- 🗺️ Mapa de calor dos estados com maior AQI
- 🏭 Gases mais críticos por região
- 📉 Ranking dos locais com piores médias de qualidade do ar

---

## 💡 Tecnologias Utilizadas

- **Python 3**
- **Pandas, Seaborn, Matplotlib, Plotly**
- **JupyterLab**
- **Docker & Docker Compose**

---

## 🧠 Aprendizados

- Criação de ambientes reprodutíveis com Docker
- Manipulação de grandes volumes de dados com pandas
- Tratamento de valores ausentes com lógica condicional
- Visualização de dados ambientais em múltiplas dimensões
- Geração automatizada de mapas e gráficos salvos como imagens

---

## 👨‍💻 Autor

Carlos Soares  
[LinkedIn](https://www.linkedin.com/in/carlos1995soares/) | [GitHub](https://github.com/carlos95soares)

---

## 📦 Imagem Docker

Disponível no Docker Hub:  
[`carlos95soares/projetodocker`](https://hub.docker.com/r/carlos95soares/projetodocker)
