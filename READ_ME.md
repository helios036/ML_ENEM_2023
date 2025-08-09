# Modelo de estimação de notas do ENEM 2023

## Objetivo do modelo

### Este repositório contém um modelo de machine learning desenvolvido para estimar as notas do ENEM 2023 com base em dados demográficos e socioeconômicos dos participantes. O foco inicial é no estado de Goiás, utilizando o algoritmo XGBoost para prever as notas nas diferentes áreas do exame.

## Delimitação do modelo

### O modelo refere-se as notas do ENEM 2023 para o estado de Goiás, com base em dados coletados pelo INEP. O objetivo é analisar como variáveis como idade, gênero, renda familiar e escolaridade dos pais influenciam o desempenho dos estudantes.

## Contextualização do problema

### O Exame Nacional do Ensino Médio (ENEM) é uma das principais formas de avaliação educacional no Brasil, influenciando o acesso ao ensino superior. Compreender os fatores que impactam o desempenho dos estudantes pode ajudar a identificar desigualdades e orientar políticas educacionais.

### O Exame Nacional do Ensino Médio (ENEM) é uma das principais formas de avaliação educacional no Brasil, influenciando o acesso ao ensino superior. Compreender os fatores que impactam o desempenho dos estudantes pode ajudar a identificar desigualdades e orientar políticas educacionais.

### Neste contexto, é fundamental analisar como variáveis demográficas e socioeconômicas influenciam as notas dos participantes. Este modelo visa fornecer insights valiosos para educadores, formuladores de políticas e pesquisadores interessados em melhorar a qualidade da educação no país.

## Gerenciamento de dados  

### Os dados utilizados neste projeto foram obtidos do [INEP](https://www.gov.br/inep/pt-br/areas-de-atuacao/avaliacao-e-exames-educacionais/enem) e incluem informações detalhadas sobre os participantes do ENEM 2023, como idade, gênero, renda familiar, nível de escolaridade dos pais, entre outros. O pré-processamento dos dados envolveu a limpeza, transformação e seleção das variáveis mais relevantes para a modelagem.

### Em relação a amostra utilizada foram considerados participantes do ENEM 2023 que residem no estado de Goiás, que estavama presentes em todas as provas do ENEM 2023, incluindo Linguagens e Códigos, Matemática, Ciências Humanas e Ciências da Natureza, que responderam o questionário socioeconômico e que tiveram suas notas divulgadas pelo INEP e que não apresentaram notas zeradas ou faltantes.

### A análise exploratória dos dados foi realizada para entender a distribuição das notas e a correlação entre as variáveis, utilizando visualizações gráficas e estatísticas descritivas.

### Os dados passaram por transformações, incluindo normalização e codificação de variáveis categóricas, para garantir a compatibilidade com o algoritmo XGBoost.

### Outro ponto de transformação de dados foi a utilização da média das provas do ENEM 2023, que foi calculada como a média aritmética das notas obtidas nas provas de Linguagens e Códigos, Matemática, Ciências Humanas e Ciências da Natureza. Essa média foi utilizada como variável alvo para o modelo de machine learning.

### Além das variaveis contidas no questionário socioeconômico, foram adicionadas variáveis externas, como o Índice de Desenvolvimento Humano (IDH) do município de residência dos participantes e o percentual de uso do programa Bolsa Familia no ano de 2023, para enriquecer a análise.

### Para selecionar as amostras mais relevantes foi utilizada a técnica SelectKBest, que ajudou a identificar as variáveis com maior impacto nas notas do ENEM. 

## Estrutura do Repositório
- `ML_ENEM_GO_2023_XGB.ipynb`: Notebook principal com todo o código e análises.
- `data/`: Diretório contendo os dados brutos e processados.