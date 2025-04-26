# 📊 Análise de Teste A/B: Estratégias A e B

Este projeto realiza a comparação entre duas estratégias de sucesso (A e B) utilizando o **Teste Z** para diferenças de médias em amostras independentes.

O objetivo é testar a hipótese nula de que **não há diferença significativa** entre as duas estratégias.

---

## 🔍 Sobre o Projeto

O código realiza:

- 📈 Cálculo das variâncias amostrais
- 🧮 Cálculo da estatística de teste Z
- 📊 Cálculo do **p-valor** associado
- 🚦 Decisão estatística com base no nível de significância de 5%

Este teste é útil para avaliar se uma nova estratégia apresenta resultados significativamente diferentes em comparação com uma estratégia já existente.

---

## 🛠️ Tecnologias Utilizadas

- **Python 3.10+** 🐍
- **Bibliotecas:**
  - [`scipy`](https://scipy.org/) — para funções estatísticas
  - `numpy` (opcional, para manipulação de arrays)
  - `pandas` (opcional, se as amostras forem DataFrames)

---

## 📈 Estrutura do Projeto
📁 Analise-Teste-Z ├── 📄 README.md ├── 📄 analise_teste_z.ipynb └── 📄 requirements.txt (opcional)

---
## 🧠 Conceitos Envolvidos

Estatística Z:
Mede a diferença entre duas médias, levando em consideração as variações amostrais.

p-valor:
Indica a probabilidade dos resultados observados ocorrerem sob a hipótese nula.

Teste Bilateral:
Testa se há diferença, sem especificar uma direção (maior ou menor).

---

## ⚡ Exemplo de Interpretação

Se o p-valor < 0.05 → Rejeitamos a hipótese nula (há diferença significativa).

Se o p-valor ≥ 0.05 → Não rejeitamos a hipótese nula (não há evidência suficiente de diferença).

---

## 🧑‍💻 Autor

Larissa Barros
