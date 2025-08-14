# Microclima da Caatinga frente às Mudanças Climáticas:  o caso do Parque Nacional Serra da Capivara (Piauí - Brasil).

Análise exploratória (EDA) de dados de temperatura e umidade



## 📑 Materiais e Métodos

### 🔹 Coleta e preparação dos dados
 O método de coleta dos dados foi feito com dataloggers da marca Akso modelo 172, foram registrados durante o período de estudo a cada hora a temperatura em graus celsius (ºC) e umidade relativa do ar (%).

### 🔹 Ferramentas
- **Python** → processamento e análise
- **pandas** → manipulação de dados
- **matplotlib** e **seaborn** → visualização gráfica

O código completo, assim como os gráficos e tabelas está disponível em:  
(https://github.com/GustavoNess/analise-exploratoria-temperatura-umidade/blob/main/EDA_temperatura_umidade.ipynb.ipynb)

---

## 📈 Principais Análises

### 1️⃣ Estatísticas anuais
- Máximo, mínimo, média, percentis 5 e 95.
- Frequência de dias extremos:
  - **Dia quente** → temperatura diária média > P95
  - **Dia frio** → temperatura diária média < P5

📌 **Tabela 1** – Estatísticas anuais de temperatura (°C)  
📌 **Tabela 2** – Estatísticas anuais de umidade (%)

---

### 2️⃣ Identificação de outliers e extremos mensais
- **Outliers** → definidos pelo intervalo interquartílico (IQR)
- **Extremos** → definidos pelos percentis 5 e 95
- Representação no boxplot:
  - 🔴 Vermelho → extremos
  - 🟡 Amarelo → outliers

📊 **Figura 1** – Distribuição mensal de temperatura  
📊 **Figura 2** – Distribuição mensal de umidade



---

### 3️⃣ Variação horária da temperatura
- Diferença entre valores máximos e mínimos para cada hora e mês
- Visualização em **heatmap**

📊 **Figura 3** – Heatmap de variação horária de temperatura (°C)

---

## 📌 Resultados e Interpretação
- Tendência de **aumento gradual** das temperaturas máximas, mínimas e médias (2022–2025)
- Aumento de amplitude térmica em meses específicos, com destaque para outubro de 2024
- Grande variabilidade de umidade (15–96%), com períodos secos e úmidos alternados
- Implicações para a preservação da arte rupestre:
  - Dilatação/contração térmica das rochas
  - Expansão/retração mineral devido à umidade

---

## 📷 Gráficos e Tabelas
As figuras e tabelas geradas estão disponíveis na pasta [`figures/`](figures/).  
Exemplo de inclusão no Markdown:

![Boxplot Temperatura](figures/boxplot_temperatura.png)
![Heatmap Variação Horária](figures/heatmap_variacao_horaria.png)

---

## 📜 Licença
Este projeto está licenciado sob a **Apache License 2.0** – veja o arquivo [LICENSE](LICENSE) para mais detalhes.  
Você pode usar e modificar o código, desde que mantenha o devido **crédito ao autor**.

---
