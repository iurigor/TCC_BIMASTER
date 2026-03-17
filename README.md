# Predição de Séries Temporais Intraday de Ações Utilizando Redes Neurais Profundas: Uma Abordagem com LSTM e Transformers com Time2Vec Aplicada à PETR4

#### Aluno: [Igor de Moraes Ferreira](https://github.com/iurigor).
#### Orientadora: [Manoela kohler](https://github.com/manoelakohler).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

---

### Resumo

Este trabalho tem como objetivo investigar o uso de técnicas de aprendizado profundo para a predição de séries temporais financeiras intraday, utilizando dados da ação PETR4 negociada na bolsa brasileira. A proposta consiste na aplicação e comparação de modelos baseados em Redes Neurais Recorrentes do tipo Long Short-Term Memory (LSTM) e arquiteturas baseadas em Transformers enriquecidas com codificação temporal por meio do método Time2Vec.

Foram utilizados dados históricos de preços de fechamento em intervalos de 15 minutos, juntamente com variáveis derivadas, como indicadores técnicos e componentes cíclicos intraday, incluindo transformações senoidais da hora de negociação. O processo de modelagem envolveu etapas de pré-processamento, normalização dos dados, criação de janelas temporais de entrada e definição de horizontes de previsão de curto prazo.

Os modelos foram avaliados com base em métricas tradicionais de regressão, além da acurácia direcional e do coeficiente de informação. Os resultados indicaram que o modelo LSTM apresentou desempenho superior em relação ao Transformer, com previsões mais estáveis ao longo do horizonte analisado. Observou-se que o erro tende a aumentar progressivamente conforme o horizonte de previsão se amplia, especialmente no modelo recorrente, enquanto o modelo baseado em Transformer apresentou maior instabilidade e erros elevados desde os primeiros passos de previsão.

Apesar de ambos os modelos apresentarem elevada correlação entre os valores previstos e reais, a acurácia direcional manteve-se próxima ao nível aleatório, evidenciando a dificuldade dos modelos em antecipar corretamente a direção dos movimentos de preço. Os resultados reforçam as limitações das abordagens testadas na modelagem de séries temporais financeiras intraday, caracterizadas por elevado nível de ruído e baixa previsibilidade, indicando que o aumento da complexidade dos modelos não necessariamente resulta em ganhos de desempenho.

---

Matrícula: 252.100.428

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
