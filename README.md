# **Previsão de Carga em Estaca Hélice Contínua com Redes Neurais Artificiais**
## Descrição

Este projeto visa o desenvolvimento de uma ferramenta preditiva baseada em Redes Neurais Artificiais (RNA) para a previsão de cargas de fuste e ponta em estacas hélice contínua. O método foi criado utilizando dados de provas de carga com células bidirecionais de estacas executadas em diferentes estados do Brasil, com o objetivo de melhorar a precisão e a confiabilidade na determinação de cargas dessas estacas.

## Metodologia

O modelo de RNA foi desenvolvido com base em um conjuntos de dados com Provas de Carga com Célula Bidirecional (PCEB). O banco de dados composto por 257 estacas de 11 estados do Brasil.
   
A otimização da rede neural foi realizada utilizando a Otimização Bayesiana para selecionar o melhor conjunto de hiperparâmetros. O modelo final foi avaliado utilizando tanto os dados de PCEB quanto os de PCEC para comparar a performance em relação a métodos convencionais amplamente usados no Brasil.
Dados de Entrada

Os dados utilizados para treinamento da RNA foram:

    Geometria da Estaca: Diâmetro e comprimento.
    NSPT (Standard Penetration Test): Média de quatro seções do fuste e o valor do NSPT para a ponta da estaca.
## Comece Aqui

Bem-vindo ao projeto de **Previsão de Carga em Estaca Hélice Contínua**! Este repositório contém uma ferramenta baseada em **Redes Neurais Artificiais (RNA)** para prever cargas de fuste e ponta em estacas hélice contínuas.

### Instruções

1. **Modelo de Arquivo CSV**: Um arquivo `.csv` modelo está disponível neste repositório. Você pode utilizá-lo como base para formatar seus dados de entrada. Certifique-se de preencher as informações necessárias, como diâmetro, comprimento, e dados de NSPT. Não mude os dados de lugar na planilha!

2. **Execução do Código**: Após preencher o arquivo `.csv`, execute o código Python contido neste repositório. O programa irá processar os dados fornecidos e realizar as previsões. Será necessário baixar o arquivo .h5 com a RNA treinada para execução do código.

3. **Relatório em PDF**: Ao final da execução do programa, um relatório em PDF será gerado automaticamente. Este relatório incluirá todas as informações que você forneceu, além dos dados da análise e das previsões de carga de fuste e ponta.


## Arquitetura da RNA

    Número de Camadas: A rede neural utilizada possui três camadas intermediárias.
    Função de Perda: A função de perda escolhida foi o Erro Absoluto Médio (MAE), que demonstrou resultados superiores comparado a outras funções de perda.

## Comparação com Métodos Convencionais

Os resultados da RNA foram comparados na tese com os métodos tradicionais brasileiros

    Décourt-Quaresma (1978)
    Aoki e Velloso (1975)

A RNA apresentou uma correlação significativamente melhor com os dados de carga, mesmo quando testada com dados de provas de carga de natureza distinta (PCEC).

## Análise de Sensibilidade

O estudo revelou que parâmetros geométricos, como diâmetro e comprimento, têm grande impacto na previsão das cargas de fuste e ponta. Por outro lado, a variação do NSPT mostrou ser sensível ao método de aplicação da carga durante as provas.

## Relatórios e Resultados

    Relatório HTML: relatorio_resultados.html
    Relatório PDF: relatorio_resultados.pdf

## Tecnologias Utilizadas

    Python 3.x
    TensorFlow/Keras: Para a implementação e treinamento da rede neural.
    Bayesian Optimization: Para otimização dos hiperparâmetros da RNA.
    Matplotlib: Para a geração de gráficos dos resultados.
    Pandas: Para manipulação e análise dos dados.
    ReportLab: Para a geração de relatórios em PDF.

## Contribuição

Este projeto faz parte de uma pesquisa acadêmica e está aberto para melhorias. Caso queira contribuir, por favor, entre em contato.

## Licença
Este projeto está licenciado sob a MIT License.
