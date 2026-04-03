# Predição de Séries Temporais Intraday de Ações Utilizando Redes Neurais Profundas: Uma Abordagem com LSTM e Transformers com Time2Vec Aplicada à PETR4

#### Aluno: [Igor de Moraes Ferreira](https://github.com/iurigor).
#### Orientadora: [Manoela kohler](https://github.com/manoelakohler).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

- LeituraDados.ipynb
- LSTM.ipynb
- Transformer.ipynb

---

### Resumo

Este projeto explora maneiras de prever o comportamento das ações da Petrobras (PETR4) ao longo do dia, usando dados de intervalos de 15 minutos. O objetivo foi comparar duas abordagens modernas: as redes LSTM, que são boas para entender sequências, e os Transformers, que usam mecanismos de atenção para captar padrões. Para ajudar, incluímos um método que ensina o modelo a perceber como o tempo se repete durante o pregão. Os resultados mostraram que, apesar de conseguirem acompanhar o movimento dos preços, acertar se a ação vai subir ou descer no próximo intervalo ainda é um grande desafio. No final, a LSTM se saiu melhor, mostrando mais estabilidade, enquanto o Transformer foi mais sensível às variações do mercado.

### Abstract

This project explores ways to predict the behavior of Petrobras (PETR4) stocks throughout the day, using 15-minute interval data. The goal was to compare two modern approaches: LSTM networks, which are good at understanding sequences, and Transformers, which use attention mechanisms to spot patterns. To help the models, we included a method that teaches them how time repeats itself during the trading session. The results showed that, although the models could follow the general movement of prices, predicting whether the stock would go up or down in the next interval is still a big challenge. In the end, the LSTM performed better, showing more stability, while the Transformer was more sensitive to market fluctuations.

### 1. Introdução

Tentar prever o mercado de ações ao longo do dia é uma tarefa complicada. Os preços mudam o tempo todo, influenciados por notícias, política e outros fatores imprevisíveis, o que gera muito ruído nos dados. Modelos antigos, como o ARIMA, costumam falhar porque simplificam demais essa realidade. Com o avanço das redes neurais, surgiu a ideia de usar essas novas ferramentas para tentar encontrar padrões nos dados históricos da PETR4. O foco aqui foi entender se aumentar a complexidade do modelo realmente traz resultados melhores em um ambiente tão instável quanto a bolsa brasileira.

### 2. Modelagem

O projeto começou com a coleta de dados via MetaTrader5, cobrindo o período de 2023 a 2026. Para dar mais contexto ao modelo, além do preço da ação, também foram usados dados do Petróleo Brent e indicadores técnicos como RSI e médias móveis. Um diferencial foi o tratamento do horário: usamos cálculos para mostrar ao modelo que certos padrões se repetem ao longo do dia. O treinamento foi feito com janelas deslizantes, onde o modelo analisava os últimos 5 dias para prever o próximo dia inteiro (28 intervalos de 15 minutos). Testamos duas arquiteturas: uma LSTM Bidirecional, que olha para os dados em ambos os sentidos, e um Transformer, que foca nos pontos mais importantes da série histórica. Todos os dados foram normalizados para facilitar o treinamento.

### 3. Resultados

Nos testes, ambos os modelos conseguiram acompanhar a tendência dos preços, mostrando alta correlação. Mas, quando o objetivo era acertar se o preço ia subir ou descer, o desempenho ficou próximo ao de um chute, entre 50% e 52%. Isso mostra como é difícil prever movimentos de curto prazo no mercado. Comparando os dois, a LSTM foi mais robusta e suas previsões foram mais estáveis. O Transformer, apesar de ser mais sofisticado, acabou se perdendo com o excesso de ruído, tentando encontrar padrões onde não havia.

### 4. Conclusões

O estudo mostrou que, no mercado financeiro, modelos mais complexos nem sempre são melhores. A LSTM, mais simples, se saiu melhor que o Transformer, principalmente por ser mais estável diante das oscilações do mercado. Para próximos estudos, talvez seja interessante incluir outros tipos de dados, como notícias ou fluxo de ordens em tempo real. A tecnologia tem potencial para ajudar na tomada de decisão, mas, para intervalos tão curtos, entender a natureza imprevisível dos preços ainda é fundamental.

---

Matrícula: 252.100.428

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
