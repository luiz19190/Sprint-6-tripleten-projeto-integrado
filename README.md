# 🎮 Video Game Sales Analysis para Sprint 6 da Tripleten: projeto integrado

> Análise exploratória de dados do mercado global de videogames — plataformas, gêneros, regiões e o que realmente impulsiona as vendas.

---

## 📌 Sobre o Projeto

Este projeto realiza uma análise completa do dataset de vendas de videogames, cobrindo mais de **16.000 jogos** lançados entre os anos 1980 e 2016. O objetivo é entender os padrões de mercado, identificar plataformas e gêneros lucrativos, comparar preferências regionais e testar hipóteses estatísticas sobre avaliações de usuários.

---

## 🗂️ Dataset

| Coluna | Descrição |
|---|---|
| `name` | Nome do jogo |
| `platform` | Plataforma de lançamento |
| `year_of_release` | Ano de lançamento |
| `genre` | Gênero do jogo |
| `na_sales` | Vendas na América do Norte (milhões) |
| `eu_sales` | Vendas na Europa (milhões) |
| `jp_sales` | Vendas no Japão (milhões) |
| `other_sales` | Vendas em outras regiões (milhões) |
| `critic_score` | Nota média dos críticos |
| `user_score` | Nota média dos usuários |
| `rating` | Classificação ESRB |

---

## 🔧 Etapas do Projeto

### 1. Pré-processamento
- Padronização dos nomes das colunas com `.str.lower()`
- Conversão de tipos: `user_score` para `float`, `year_of_release` para `Int64`
- Tratamento de valores ausentes (`critic_score`, `user_score`, `rating`)
- Criação da coluna `total_sales` (soma de todas as regiões)

### 2. Análise de Plataformas
- Identificação das plataformas com maiores vendas totais
- Análise do ciclo de vida das plataformas (surgimento e declínio)
- Correlação entre avaliações e vendas por plataforma

### 3. Análise de Gêneros
- Distribuição de jogos por gênero
- Comparação entre volume total e vendas médias por gênero
- Identificação dos gêneros mais lucrativos

### 4. Análise Regional
- Top 5 plataformas por região (NA, EU, JP)
- Top 5 gêneros por região
- Impacto da classificação ESRB nas vendas regionais

### 5. Testes de Hipótese
- Teste t de Student para comparação de médias
- Xbox One vs PC: avaliações médias de usuários
- Action vs Sports: avaliações médias de usuários

---

## 📊 Principais Descobertas

- **Action** lidera em volume total de vendas, mas **Platform** tem a maior média por jogo — sustentada por franquias como Mario e Sonic
- As avaliações de **críticos** têm correlação moderada com vendas (0.39), enquanto as de **usuários** praticamente não influenciam (0.11)
- O **Japão** tem preferências bem distintas de NA e EU, com forte preferência por plataformas japonesas e RPGs
- Estatisticamente, Xbox One e PC possuem avaliações médias **diferentes** (p ≈ 0), enquanto Action e Sports **não diferem** significativamente (p > 0.1)

---

## 🛠️ Tecnologias Utilizadas

+ **Python**
+ **Pandas**
+ **Matplotlib**
+ **SciPy**
+ **Jupyter**
+ **Vs code**
+ **Claude**

---

## 📁 Estrutura do Projeto

```
├── games.csv                  # Dataset original
├── notebook.ipynb             # Análise completa em Jupyter
├── README.md                  # Este arquivo
└── graficos/
    ├── platform_sales.png     # Vendas por plataforma
    ├── genre_analysis.png     # Análise por gênero
    ├── score_vs_sales.png     # Avaliações vs vendas
    ├── top_plataformas.png    # Top plataformas por região
    ├── top_generos.png        # Top gêneros por região
    └── esrb_rating.png        # ESRB por região
```

---

## 👤 Autor

Feito com 🎮 e muito `pandas` por **[Luiz Trajano]**  
[

![GitHub](https://img.shields.io/badge/GitHub-luiz19190-181717?style=flat&logo=github)

](https://github.com/luiz19190/Sprint-6-tripleten-projeto-integrado)

