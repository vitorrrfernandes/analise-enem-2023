# 📊 Análise Exploratória — Microdados ENEM 2023

> Investigando como **renda familiar**, **região** e **tipo de escola** se relacionam com o desempenho dos candidatos no ENEM 2023.

---

## 📌 Sobre o Projeto

Este projeto realiza uma **Análise Exploratória de Dados (EDA)** sobre os microdados oficiais do ENEM 2023, disponibilizados pelo INEP. O objetivo é identificar padrões de desempenho entre diferentes grupos socioeconômicos e regionais, respondendo a perguntas concretas sobre desigualdade educacional no Brasil.

É o primeiro projeto do meu portfólio de dados, desenvolvido como parte da minha transição de carreira para a área de dados.

---

## ❓ Perguntas Investigadas

1. **Existe diferença na nota média entre faixas de renda familiar?**
2. **Quais estados (UF) apresentam maior e menor desempenho médio?**
3. **Alunos de escolas privadas têm desempenho significativamente maior que os de escolas públicas?**

---

## 🔍 Principais Achados

### 1. Renda Familiar × Desempenho
- Há uma relação **diretamente proporcional e consistente** entre renda e nota em todas as 5 áreas do exame
- Candidatos na faixa mais baixa (A — até R$ 1.412) obtêm nota geral média em torno de **480 pontos**
- Candidatos na faixa mais alta (Q — acima de R$ 28.240) ultrapassam **650 pontos**
- Diferença total entre extremos: **mais de 150 pontos** na nota geral

### 2. Desempenho por Estado (UF)
- Estados do **Sudeste e Sul** (DF, SP, MG, SC, RS) lideram o ranking de notas
- Estados do **Norte e Nordeste** (AM, AP, MA) concentram os menores desempenhos
- A diferença entre o estado com maior e menor média supera **80 pontos**, evidenciando forte desigualdade regional

### 3. Escola Pública × Privada
- Alunos de **escolas privadas** apresentam nota geral média ~**616 pontos**
- Alunos de **escolas públicas** apresentam nota geral média ~**516 pontos**
- Diferença de aproximadamente **100 pontos** — equivalente a quase um desvio padrão

> ⚠️ **Nota metodológica:** estas análises são descritivas. As variáveis (renda, tipo de escola, UF) são altamente correlacionadas entre si — não foi realizado controle estatístico para isolar o efeito individual de cada fator.

---

## 🛠️ Tecnologias Utilizadas

| Ferramenta | Uso |
|---|---|
| Python 3 | Linguagem principal |
| Pandas | Manipulação e análise dos dados |
| Matplotlib | Visualização de dados |
| Seaborn | Visualização estatística |
| Jupyter Notebook | Ambiente de desenvolvimento |

---

## 📁 Estrutura do Repositório

```
analise-enem-2023/
├── analise_enem_2023.ipynb   # Notebook principal com toda a análise
├── README.md                 # Este arquivo
└── .gitignore                # Exclui o CSV (muito grande para o GitHub)
```

---

## ▶️ Como Reproduzir

**1. Clone o repositório**
```bash
git clone https://github.com/vitorrrfernandes/analise-enem-2023.git
cd analise-enem-2023
```

**2. Instale as dependências**
```bash
pip install pandas matplotlib seaborn jupyter
```

**3. Baixe o dataset**

O arquivo CSV não está incluído no repositório por conta do tamanho (441MB). Baixe os microdados diretamente no Kaggle:

🔗 [ENEM 2023 - Microdados (Kaggle)](https://www.kaggle.com/datasets)

Após baixar, coloque o arquivo `MICRODADOS_ENEM_2023_trabalhado.csv` na mesma pasta do notebook.

**4. Execute o notebook**
```bash
jupyter notebook analise_enem_2023.ipynb
```

Execute as células em ordem (`Run All` ou `Shift+Enter` em cada célula).

---

## 👤 Autor

**Vitor Fernandes**
Estudante de Sistemas de Informação — UFG

[![GitHub](https://img.shields.io/badge/GitHub-vitorrrfernandes-181717?style=flat&logo=github)](https://github.com/vitorrrfernandes)

---

*Dados públicos do INEP — Ministério da Educação. Este projeto tem fins exclusivamente educacionais.*
