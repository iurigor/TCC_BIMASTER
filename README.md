# Título do Trabalho

#### Alun(o/a): [Igor de Moraes Ferreira](https://github.com/iurigor).
#### Orientador(/a/es/as): [Manoela kohler](https://github.com/manoelakohler).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

---

### Resumo

Este trabalho tem como objetivo investigar o uso de técnicas de aprendizado profundo para a predição de séries temporais financeiras intraday, utilizando dados da ação PETR4 negociada na bolsa brasileira. A proposta consiste na aplicação e comparação de modelos baseados em Redes Neurais Recorrentes do tipo Long Short-Term Memory (LSTM) e arquiteturas baseadas em Transformers enriquecidas com codificação temporal por meio do método Time2Vec.

Foram utilizados dados históricos de preços de fechamento em intervalos de 15 minutos, juntamente com variáveis derivadas, como indicadores técnicos e componentes cíclicos intraday, incluindo transformações senoidais da hora de negociação. O processo de modelagem envolveu etapas de pré-processamento, normalização dos dados, criação de janelas temporais de entrada e definição de horizontes de previsão de curto prazo.

Os modelos foram avaliados com base em métricas tradicionais de regressão, como erro médio absoluto (MAE) e erro quadrático médio (RMSE), além da acurácia direcional, considerada particularmente relevante no contexto financeiro. A incorporação do Time2Vec permitiu ao modelo Transformer capturar padrões temporais periódicos de forma mais eficiente, enquanto o modelo LSTM serviu como baseline para comparação de desempenho.

Os resultados indicam que arquiteturas baseadas em atenção, quando combinadas com representações temporais adequadas, apresentam potencial para capturar dinâmicas complexas do mercado intraday. No entanto, destaca-se a dificuldade inerente à previsão de preços financeiros, caracterizados por alta volatilidade e baixo sinal preditivo. Ainda assim, observa-se ganho incremental na acurácia direcional em comparação com abordagens tradicionais, sugerindo a viabilidade do uso dessas técnicas em apoio à tomada de decisão no mercado financeiro.

---

Matrícula: 252.100.428

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
