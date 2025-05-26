# 🔍 Detecção de Fraudes Financeiras – PaySim

Este projeto utiliza um conjunto de dados **simulado** de transações financeiras (PaySim) com o objetivo de **detectar fraudes** por meio de técnicas de Machine Learning.

---

## 🧪 ETL (Extração, Transformação e Carga)

- Tratamento de dados faltantes.
- Conversão de tipos de dados.
- Criação de uma nova coluna para identificar o tipo de cliente:
  - `C` para **CPF** (Pessoa Física)
  - `M` para **CNPJ** (Pessoa Jurídica)

---

## 📊 Visualização de Dados

As variáveis com maior influência na predição de fraude foram identificadas por meio de gráficos de **barras** e **boxplot**:

- Hora da transação
- Valor da transação
- Tipo de destino (CPF ou CNPJ)

---

## 🕵️‍♂️ Perfil Comum das Transações Fraudulentas

- Tipo de cliente: **CPF** (Pessoa Física)
- Horário mais recorrente: **00:00h**
- Valor médio das fraudes: **R$ 500.000**
- Destino: Conta de pessoa física (**CPF**)

---

## 🤖 Aprendizado Supervisionado

**Modelos utilizados:**

- 🌳 Árvore de Decisão – Acurácia: **99,97%**
- 📈 Regressão Logística – Acurácia: **99,99%**

> O modelo de **Regressão Logística** apresentou melhor desempenho e foi **encapsulado** para uso posterior na aplicação.

---

## 🚀 Aplicação

- Interface simples desenvolvida com **Gradio**
- O usuário insere os dados da transação e o sistema retorna a **probabilidade de fraude**

---

## 📂 Fonte dos Dados

- Dataset disponível em:  
  [🔗 Kaggle - PaySim Fraud Detection Dataset](https://www.kaggle.com/datasets/ealaxi/paysim1/data)  
  *Simulação baseada em transações reais de Mobile Money, com foco em detecção de fraudes.*
