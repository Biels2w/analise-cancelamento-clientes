# Análise de Cancelamento de Clientes (Churn)

Análise exploratória de dados para identificar os principais motivos de cancelamento de clientes de uma empresa com uma base de mais de 800 mil usuários, e propor ações para reduzir a taxa de churn.

## 📋 Sobre o projeto

Uma empresa percebeu que a maior parte da sua base de clientes está inativa, ou seja, já cancelou o serviço. O objetivo deste projeto é entender **por que** os clientes estão cancelando e quais fatores mais influenciam essa decisão, para sugerir ações práticas de retenção.

## 🔍 O que foi feito

- Leitura e tratamento da base de dados (remoção de colunas irrelevantes e valores nulos)
- Análise exploratória com gráficos (histogramas) para cada variável, cruzando com a taxa de cancelamento
- Identificação dos principais fatores associados ao cancelamento:
  - **Tipo de contrato**: clientes com contrato mensal apresentam taxa de cancelamento muito acima da média
  - **Ligações para o call center**: mais de 4 ligações aumenta fortemente a chance de cancelamento
  - **Atraso no pagamento**: mais de 20 dias de atraso também está associado a maior churn
- Simulação do impacto de ações de retenção (ex: migrar clientes do plano mensal, reduzir atrasos e chamadas ao suporte) na redução da taxa de cancelamento

## 📊 Resultado

A taxa inicial de cancelamento da base era de aproximadamente 56%. Ao simular a remoção dos clientes nos grupos de risco (contrato mensal, muitas ligações ao call center, atrasos longos), a taxa projetada cai para cerca de 18%, mostrando o forte impacto desses três fatores.

## 🛠️ Tecnologias utilizadas

- Python
- Pandas — leitura e manipulação dos dados
- Plotly Express — visualização de dados

## 📁 Estrutura do projeto

```
├── inicial.ipynb          # Notebook com toda a análise
├── cancelamentos.csv       # Base de dados utilizada
└── README.md
```

## ▶️ Como executar

1. Clone o repositório
```bash
git clone https://github.com/SEU_USUARIO/analise-cancelamento-clientes.git
```

2. Crie um ambiente virtual e instale as dependências
```bash
python -m venv venv
venv\Scripts\activate  # Windows
pip install pandas plotly ipykernel nbformat
```

3. Abra o `inicial.ipynb` no VS Code ou Jupyter e execute as células

## 📌 Próximos passos

- Testar modelos preditivos (ex: regressão logística, árvore de decisão) para prever cancelamento
- Aprofundar a análise por segmento de cliente (idade, tipo de assinatura)

---

Projeto desenvolvido como parte de estudos em análise de dados com Python.
