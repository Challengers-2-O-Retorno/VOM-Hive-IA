
# Vom - Hive - Inteligência Artificial

A inteligência artificial da VOM - Hive tem como objetivo, com base em análises de campanhas de marketing e seus metadados, determinar qual a melhor rede social para criar uma campanha de marketing. Este protótipo funcional foi desenvolvido para testes e pode ser utilizado para validar estratégias de marketing digital de forma prática.

Os dados analisados incluem informações como público-alvo, objetivo da campanha, duração, taxa de conversão, custo de aquisição, retorno sobre investimento (ROI), localização, idioma, cliques, impressões, engajamento, e outros fatores. Com base nesses dados, foi desenvolvido um modelo de Machine Learning utilizando o algoritmo Random Forest Classifier.

Este protótipo funcional realiza previsões baseadas nas características de campanhas passadas, ajudando a identificar a rede social com maior potencial de sucesso para novas campanhas. Ele oferece uma solução prática e eficiente para empresas que buscam otimizar suas campanhas de marketing digital, possibilitando uma tomada de decisão mais assertiva.



## Detalhamento da Arquitetura de IA
1. Coleta e Pré-processamento de Dados
Fonte dos dados: Os dados utilizados foram coletados de campanhas de marketing em redes sociais, abrangendo características como:
Público-alvo (Target_Audience)
Meta da campanha (Campaign_Goal)
Duração (Duration)
Canal utilizado (Channel_Used)
Taxa de conversão (Conversion_Rate)
Custo de aquisição (Acquisition_Cost)
Retorno sobre investimento (ROI)
Engajamento (Engagement_Score)
Cliques e impressões, entre outros.
Pré-processamento:
Codificação de variáveis categóricas: Variáveis categóricas como "Target_Audience" e "Campaign_Goal" foram convertidas em numéricas usando OneHotEncoder e LabelEncoder.


2. Divisão dos Dados
Os dados foram divididos em conjuntos de treino e teste, seguindo a prática comum de usar aproximadamente 80% para treino e 20% para teste.
Utilizou-se também a validação cruzada (k-fold) para garantir que o modelo fosse avaliado de forma consistente em diferentes partições dos dados.


3. Treinamento do Modelo
Algoritmo utilizado: O modelo foi construído utilizando o algoritmo Random Forest Classifier, que é uma técnica baseada em árvores de decisão. O Random Forest é uma técnica de ensemble, onde múltiplas árvores de decisão são criadas, e suas previsões são combinadas para melhorar a precisão do modelo.

        Justificativa: O Random Forest foi escolhido por sua capacidade de lidar com grandes quantidades de dados, suas boas propriedades para classificação e sua robustez contra overfitting. Ele também lida bem com variáveis mistas (numéricas e categóricas) e consegue identificar interações complexas entre as variáveis.

4. Avaliação do Modelo
A avaliação do desempenho do modelo foi realizada utilizando o conjunto de dados de teste para gerar as predições do modelo treinado. O desempenho das predições foi então analisado por meio de um relatório de classificação que apresentou métricas detalhadas sobre a precisão do modelo.

O relatório incluiu as seguintes métricas principais:

- **Precisão** (Precision): Indicando a porcentagem de predições corretas para cada classe (rede social) em relação ao total de predições feitas.
- **Recall** (Sensibilidade): Mostrando a capacidade do modelo em identificar corretamente as ocorrências verdadeiras de cada classe.
- **F1-Score**: Uma média entre precisão e recall, útil para equilibrar essas métricas e fornecer uma visão geral do desempenho.
- **Suporte**: Representando o número de ocorrências reais de cada classe nos dados de teste.

        Essas métricas permitiram uma análise clara da eficácia do modelo, identificando tanto suas forças quanto áreas de melhoria para futuras otimizações.

5. Implementação e Uso do Modelo
Após o treinamento e validação, o modelo pode ser utilizado para prever a melhor rede social para campanhas futuras, baseando-se nos dados históricos fornecidos.
Input do modelo: As variáveis que serão inseridas para realizar uma nova previsão incluem informações da campanha, como público-alvo, meta, duração, impressões e taxa de engajamento.
Output do modelo: O modelo retorna a previsão de qual rede social (Channel_Used) tem a maior probabilidade de gerar melhores resultados para a campanha.




## Rodando localmente

Garanta que você tenha baixado as seguintes especificações:

- [Python](https://www.python.org/downloads/)  
- [Sikit-learn](https://pypi.org/project/scikit-learn/)  
- [Pandas](https://pypi.org/project/pandas/)

Com tudo baixado agora clone o projeto

```bash
  git clone https://link-para-o-projeto
```

Entre no diretório do projeto

```bash
  cd my-project
```
Agora só rodar o arquivo `VOM-Hive-IA.ipynb` no editor que preferir


## Autores - 2TDSPF

- [@Jixatos RM551408](https://github.com/Jixatos) RM551408
- [@IsabellajFerreira](https://github.com/IsabellajFerreira) RM552329
- [@gutolive09](https://github.com/gutolive09) RM550548
- [@Mmateus106](https://github.com/Mmateus106) RM98524
- [@gabrielrodri33 RM550548](https://github.com/gabrielrodri33) RM98626