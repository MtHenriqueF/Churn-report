# 📊 Power BI Case Study – Customer Churn Analysis  

## 📌 Descrição  
Este projeto é um **estudo de caso em Power BI** utilizando dados de uma empresa fictícia de telecomunicações chamada **Databel**. O objetivo é analisar a **taxa de churn (cancelamento de clientes)** e entender os principais fatores que influenciam o desligamento.  

---
## 🛠️ Ferramentas Utilizadas  
- **Power BI Desktop** (ETL, modelagem, visualização)  
- **Power Query** (transformação de dados)  
- **DAX (Data Analysis Expressions)** (medidas e colunas calculadas)  

---

## 📂 Estrutura do Projeto  

**Importação e limpeza dos dados**  
   - Tratamento da coluna `Churn Label` (Yes/No → 1/0).  
   - Criação de colunas calculadas para análise de churn.  

**Modelagem dos dados**  
   - Criação de relacionamentos.  
   - Estruturação de medidas para cálculo da taxa de churn.  

**Criação de medidas em DAX**  
   - Total de clientes churned.  
   - Taxa de churn (%).  
   - Distribuições de churn por região, plano e tempo de assinatura.  


---

## 📊 Exemplos de Métricas Criadas  
```DAX
Total Customers = COUNTROWS('Customers')

Total Churned = CALCULATE(
    COUNTROWS('Customers'),
    'Customers'[Churned] = 1
)

Churn Rate = DIVIDE([Total Churned], [Total Customers], 0)
```

---

## 🎯 Resultados Esperados  
- **Taxa de churn clara e atualizada**.  
- **Identificação dos fatores mais críticos** para cancelamento.  
- **Dashboard interativo** para tomada de decisão estratégica.  

---


## 📌 Autor  
Projeto desenvolvido como estudo de caso em **Power BI**, aplicando técnicas de análise de dados e DAX em um cenário realista de negócio.  
