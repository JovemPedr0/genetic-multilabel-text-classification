# 📚 Classificação de Texto Multirrótulo com Classifier Chains e Algoritmo Genético

Este projeto explora e compara técnicas de **classificação multirrótulo** usando **Classifier Chains** tradicionais e uma abordagem baseada em **Algoritmos Genéticos** para otimizar a ordem dos rótulos.

## 🚀 Objetivo

Investigar se a otimização da ordem dos rótulos em Classifier Chains, utilizando Algoritmos Genéticos, pode melhorar o desempenho em tarefas de classificação de textos.

## 🛠️ Tecnologias Utilizadas

- Python 3.x
- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://numpy.org/)
- [scikit-learn](https://scikit-learn.org/stable/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)
- [tqdm](https://tqdm.github.io/)

## 📁 Estrutura dos Dados

Os dados devem estar organizados na seguinte estrutura:

```
/data
  ├── train.csv
  └── test.csv
```

Cada CSV deve conter pelo menos as colunas:
- `TITLE` — título do texto
- `ABSTRACT` — resumo ou corpo do texto
- E as colunas de **rótulos** (targets).

**Observação**: A coluna `ID`, se existir, será descartada.

## 🧩 Etapas

1. **Pré-processamento dos Dados**  
   - Remoção de colunas desnecessárias
   - Preenchimento de valores nulos
   - Vetorização de texto com **TF-IDF**

2. **Modelagem**
   - **Classifier Chain** padrão usando regressão logística
   - **Algoritmo Genético** para otimizar a ordem dos rótulos na cadeia

3. **Avaliação**
   - Métricas usadas: F1-Score, Precisão, Revocação
   - Matrizes de confusão multirrótulo

## 📈 Resultados Esperados

Comparações entre:
- Classifier Chain com ordem natural dos rótulos
- Classifier Chain com ordem otimizada via Algoritmo Genético

