# Projeto 2: Análise de Preferências Musicais

## Visão Geral

Este projeto apresenta o fluxo de trabalho de um analista de dados, desde a exploração inicial até o teste de hipóteses. Utilizando um conjunto de dados de um serviço de streaming de música, o objetivo foi analisar e comparar o comportamento dos usuários nas cidades de **Springfield** e **Shelbyville** para validar ou rejeitar uma hipótese sobre suas preferências musicais em diferentes dias da semana.

## Objetivo

Testar a seguinte hipótese:

> **"A atividade dos usuários é diferente dependendo do dia da semana e da cidade."**

## Dados

O conjunto de dados utilizado foi o `music_project_en.csv`, contendo as seguintes colunas:

- **userID**: Identificador do usuário
- **Track**: Título da música
- **artist**: Nome do artista
- **genre**: Gênero musical
- **City**: Cidade do usuário (Springfield ou Shelbyville)
- **time**: Horário em que a música foi tocada
- **Day**: Dia da semana

## Metodologia e Etapas

O projeto foi dividido em três etapas principais:

1. **Visão Geral dos Dados**  
    Exploração inicial do dataset para entender sua estrutura, tipos de dados e possíveis problemas como valores ausentes ou duplicados.

2. **Pré-processamento de Dados**  
    Limpeza e preparação dos dados para análise:
    - Renomeação das colunas para um padrão mais claro e consistente
    - Identificação e preenchimento de valores ausentes (`NaN`)
    - Verificação e remoção de linhas duplicadas

3. **Teste da Hipótese**  
    Com os dados limpos, a análise focou em validar a hipótese. Os dados foram filtrados por cidade e dia da semana, e a contagem de músicas por gênero foi agregada para comparar as preferências entre Springfield e Shelbyville na segunda-feira, quarta-feira e sexta-feira.

## Habilidades e Ferramentas Aplicadas

- **Pandas**: Manipulação de DataFrames, incluindo:
  - Leitura e exploração de dados
  - Filtragem de dados com base em condições (`df[condicao]`)
  - Tratamento de valores ausentes (`.fillna()`)
  - Detecção e remoção de duplicatas (`.duplicated()`, `.drop_duplicates()`)
  - Agrupamento e agregação de dados (`.groupby()`, `.count()`)

## Conclusão

Este projeto serviu como uma aplicação prática do processo de teste de hipóteses, demonstrando como o pré-processamento de dados é fundamental para garantir resultados analíticos confiáveis. A análise permitiu tirar conclusões sobre as diferenças e semelhanças no consumo de música entre as duas cidades, validando parcialmente a hipótese inicial.
