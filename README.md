# Classificador ESpam
 Projeto de Classificação de Spam -  2º etapa do processo seletivo.
 
 # Introdução
 
 O projeto foi realizado testando 5 Modelos de classificação, avaliando suas métricas e escolhendo o modelo de melhor perfomance.
 Foram utilizados os seguintes modelos e suas respectivas acurácias após o ajuste de parâmetros:
 
 Naive Bayes 84%, Random Forest 81%, Knn 82%, SVM 84% e Rede Neural 84%.
 O modelo escolhido foi o Naive Bayes com 84% de acurácia, pois é um modelo simples e rápido, que teve os melhores resultados entre os modelos treinados.
 
 # Etapas Iniciais do projeto: Passo 0.0 até 5.0
 
 0.0 Foi a etapa de importação 
 
 1.0 Nesta estapa foi realidada as primeiras obervações dos dados, dimensões, dados nulos e limpeza inicial dos dados
 
 2.0 Após a limpeza inicial que foi removido as pontuações, caracteres especiais, emojis e números, foi gerada nuvens de palavras para cada classe: Spam e Não Spam.Com isso podemos observar as palavras mais frenquentes em cada classe e fazer comparações. Na nuvem de mensagens spam percebemos mais gírias, palavras com conotação sexual entre outras.
 
 3.0 Nesta etapa foi realizado a modelagem dos dados passo a passo:
     - Separação das variáveis de entrada e variável target(classe: True para SPAM e False para mensagens NÃO SPAM)
     - Limpeza  dos dados com a função criada
     - Tokenização e transformação em vetor
     - TF-IDF
     - Separação dos dados tradado em treino e teste, com 20% para teste.
     
  4.0 Treinamento e avaliação dos modelos:
      - Os modelos foram treinados com parâmetros default, e apresentadas as métricas de  Precision, Recall, F1-Score e Acurácia.
 
 5.0 Nesta etapa foram testadas algumas combinações de parâmetros com a função GridSchearchCV, que já utliza a técnica Cross Validation, e selecionados 5 Folds.
 
 
# Etapas finais: Passo 6.0 e 7.0

6.0 Etapa que foi escolhido o naive bayes como modelo para criar o classificador, construção do pipeline para encapsular as etapas anteriores: limpeza, transformação e treinamento do modelo. Foi gerado o resultado final do modelo e suas métricas.

7.0 Previsões na base de teste e criação de um função ESpam para receber uma mensagem e retornar se é spam ou não. 

   
 
    
