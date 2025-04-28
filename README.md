# Classificação de Gêneros Musicais usando Random Forest

Este projeto consiste na extração e seleção de características de sinais de áudio para a classificação automática de músicas por gênero musical. Utilizando o dataset **GTZAN**, aplicamos a técnica de **Random Forest** para identificar as características mais relevantes e treinar um modelo de aprendizado de máquina.

## Integrantes

- Matheus Augusto Monte Silva - [mams4@cin.ufpe.br](mailto:mams4@cin.ufpe.br)
- Antônio Apolinário Barbosa - [aab2@cin.ufpe.br](mailto:aab2@cin.ufpe.br)
- Mariana Melo dos Santos - [mms11@cin.ufpe.br](mailto:mms11@cin.ufpe.br)

## Metodologia

- **Dataset**: Utilizamos o GTZAN, com 1000 faixas distribuídas entre 10 gêneros musicais.
- **Pré-processamento**:
  - Segmentação dos áudios em trechos de 3 segundos.
  - Sobreposição de janelas para maior preservação temporal.
  - Representação das características na escala de frequência Mel (Mel Spectrograma).
- **Extração de Características**:
  - Energia perceptual (`perceptr`), MFCCs, Transformada de Fourier, entre outras.
- **Seleção de Características**:
  - Ranking de importância gerado pelo algoritmo Random Forest.
- **Treinamento e Avaliação**:
  - Divisão de dados em 80% treino e 20% teste.
  - Acurácia de 72,26% sem ruído e 70,88% com ruído/eco adicionados.
  - Avaliação realizada também com matrizes de confusão.

## Resultados

O modelo demonstrou boa capacidade de classificação, mesmo sob condições de perturbação (ruído e eco), e permitiu a identificação de padrões acústicos importantes para a diferenciação de gêneros musicais.

## Direitos sobre o Dataset

Todos os direitos sobre o dataset **GTZAN** são reservados aos seus criadores e podem ser consultados neste link:  
🔗 [GTZAN Dataset no Kaggle](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification)

---

