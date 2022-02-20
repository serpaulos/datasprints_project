# Datasprint Desafio Tecnico


> Desafio enviao por DataSprints <br>
>![Alt text](logo.png)

## Tabela de Conteudos
- [Informações Gerais](#Informações-Gerais)
- [Tecnologias](#Tecnologias)
- [Melhorias](#melhorias)
- [Contato](#Contato)
<!-- * [License](#license) -->


## Informações-Gerais 
- Foi utilizado o conjunto de Dados disponibilizado pela empresa com base nos dados da NYC Taxi Trips.
    - data-sample_data-nyctaxi-trips-2009-json_corrigido.json
    - data-sample_data-nyctaxi-trips-2010-json_corrigido.json
    - data-sample_data-nyctaxi-trips-2011-json_corrigido.json
    - data-sample_data-nyctaxi-trips-2012-json_corrigido.json
    - data-payment_lookup-csv.csv
    - data-vendor_lookup-csv.csv

- O objetivo deste teste é avaliar sua proficiência nos requisitos básicos para nossa vaga:
    - Programação básica com SQL
    - Programação básica com Python
    - Experiência com Cloud Computing
    - Experiência com Linux
    - Experiência com Data Science/Engineering
    - Habilidades diferenciais :
        - Habilidades em Análise de Grandes Volumes de Dados;
        - Habilidades em construção de pipelines de dados.

- Queremos que, a partir dos dados disponibilizados, você responda, de preferência com gráficos às seguintes questões
    - 1. Qual a distância média percorrida por viagens com no máximo 2 passageiros;
    - 2. Quais os 3 maiores vendors em quantidade total de dinheiro arrecadado;
    - 3. Faça um histograma da distribuição mensal, nos 4 anos, de corridas pagas em dinheiro;
    - 4. Faça um gráfico de série temporal contando a quantidade de gorjetas de cada dia, nos  últimos 3 meses de 2012.

## Tecnologias
- Python
- Mysql


# Detalhes-do-Projeto

* Os arquivos JSON foram convertidos para o fomato PARQUET por ser um arquivo de tamanho menor e melhor performance.

* Dentro do arquivo desafio.ipynb podem ser encontrados anotações e detalhes a respeito das etapas realizadas, dentre elas:
    - importar as bibliotecas necessarias.
        - pandas
        - pyarrow
        - datetime
        - matplotlib
        - seaborn
        - folium
        - numpy
* Foi criada uma funcao para converter arquivos JSON de uma determinada pasta para o formato parquet, converte_parquet(), porem por ser necessario poucas comversões, foram feitas conversões manualmente

* Foi feita uma carga em banco de dados Mysql para teste e escrita de queries para consulta ao banco.
    - A carga foi feita usando sqlalchemy, usando um dataframe consolidado de todos os outros criados manualmente, utilizando este  comando para a carga
    - df_concat.to_sql('taxi_pickups', engine)
* Arquivo Análise.html foi criado/incluido no repositorio com as respostas obtidas para as perguntas.

## Contato
Criado por [@paulosilvajr](https://www.linkedin.com/in/paulosilvajr/) - fique a vontade para entrar em contato! [sergiopaulosilvajr@gmail.com](sergiopaulosilvajr@gmail.com)