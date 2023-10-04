# Processo ETL (Extract, Transform, Load)

Olá! Neste projeto, implementamos um pipeline ETL (Extract, Transform, Load) para processar dados provenientes da API JSONPlaceholder. Vamos explicar as etapas do processo ETL que realizamos:

## Extração (Extract):

Na etapa de extração, utilizei a biblioteca `requests` para fazer uma requisição GET à API JSONPlaceholder que contém dados de posts. Criei a função `extract_data()` para obter esses dados. Os dados extraídos são retornados em forma de uma lista de dicionários, representando os posts.

## Transformação (Transform):

A transformação dos dados é uma etapa essencial. Utilizei a função `transform_data()` para processar os dados extraídos. Neste exemplo, realizamos uma transformação simples, renomeando algumas colunas para padronizar os nomes e melhorar a legibilidade dos dados. Essa etapa é crucial para preparar os dados de maneira apropriada para análise e utilização futura.

## Carregamento (Load):

Para o carregamento dos dados transformados, criei a função `load_data_excel()`. Utilizei a biblioteca Pandas para salvar os dados transformados em um arquivo Excel (xlsx). A função `to_excel()` foi usada para criar o arquivo Excel a partir do DataFrame contendo os dados transformados. Escolhi o formato Excel para facilitar o compartilhamento e a visualização dos dados processados.

O processo ETL é fundamental para preparar e organizar os dados, garantindo que estejam prontos para análise e utilização de forma eficiente.
