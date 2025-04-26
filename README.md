📊 Análise de Teste A/B: Estratégias A e B
Este projeto realiza a comparação entre duas estratégias de sucesso (A e B) utilizando teste Z para diferenças de médias em amostras independentes.

O objetivo é testar a hipótese nula de que não há diferença entre as duas estratégias.

🔍 Sobre o Projeto
O código:

Calcula as variâncias amostrais 📈

Calcula a estatística de teste Z 🧮

Determina o p-valor associado a essa estatística 📊

Compara o p-valor a um nível de significância (5%) para decidir se rejeita ou não a hipótese nula 🚦

🛠️ Tecnologias Utilizadas
Python 🐍

Bibliotecas:

scipy

numpy (opcional, para trabalhar com arrays)

pandas (opcional, se suas amostras forem DataFrames)

🧩 Como Rodar o Projeto
Clone o repositório:

bash
Copiar
Editar
git clone https://github.com/seu-usuario/seu-repositorio.git
Instale as dependências:

bash
Copiar
Editar
pip install scipy numpy pandas
Execute o notebook (.ipynb) no Jupyter Notebook, Google Colab ou VSCode.

📈 Estrutura do Código
python
Copiar
Editar
# 1. Calcular variâncias
var_existente = amostra_estrategia_A.var(ddof=1)
var_novo = amostra_estrategia_B.var(ddof=1)

# 2. Calcular médias
media_existente = amostra_estrategia_A.mean()
media_novo = amostra_estrategia_B.mean()

# 3. Estatística de teste Z
z_statistic = (media_existente - media_novo) / ((var_existente/n + var_novo/n) ** 0.5)

# 4. Calcular p-valor
p_valor = 2 * (1 - stats.norm.cdf(abs(z_statistic)))

# 5. Decisão
if p_valor < 0.05:
    print("Rejeitamos a hipótese nula.")
else:
    print("Não rejeitamos a hipótese nula.")
📚 Conceitos Trabalhados
Estatística de Teste Z

Variância amostral

Teste de Hipóteses

p-valor

Nível de significância

✨ Melhorias Futuras
Implementar visualização dos resultados (gráficos comparando as duas estratégias)

Automatizar para diferentes tamanhos de amostra

Transformar em função ou classe para reuso

🧑‍💻 Autor
Larissa Barros
