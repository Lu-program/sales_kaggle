# Sales Orders - Kaggle
Esse repositório é focado em processos de Preparação, Limpeza de dados para Análise de Dados voltado para painel de Business Intelligence de Sales do portifólio do Kaggle. 

Repositório da Base Bruta do Kaggle: https://www.kaggle.com/datasets/vincentcornlius/sales-orders?resource=download

Na Base Bruta temos colunas referente a venda de produtos de varejo de mercado do setor B2C (business to consumer). Com suas relativas datas de entrega, lucro de venda por produto, 
venda de produto e local de entrega. 

O arquivo se encontra em um csv chamado: sales_data.csv 

Os arquivos de análise dos dados estão agrupados em uma pasta chamada Análise de dados_sales_csv, que contém: 

- Arquivo de: preparação_limpeza_sales_df

O objetivo desse arquivo é de analisar a presença de nulos, analisar a presença de duplicatas, verificar a classificação das categorias, ordenar as colunas, renomear as colunas para maior entendimento, estudo das categorias e seus significados, criação de novas categorias para e padronização de alguns dados internos para a análise posterior. 

Print(sales_df)

          ID                   Produto     Categoria  \
7043  147963             Flatscreen TV  Alimentation   
424   141647              20in Monitor  Électronique   
423   141646  Lightning Charging Cable  Alimentation   
3945  144994           ThinkPad Laptop  Alimentation   
420   141644    AAA Batteries (4-pack)     Vêtements   

                           Recebido(local) Recebido(cidade)  \
7043       655 Meadow St, Austin, TX 73301           Austin   
424       434 Sunset St, Atlanta, GA 30301          Atlanta   
423         678 Adams St, Dallas, TX 75001           Dallas   
3945  903 Willow St, Los Angeles, CA 90001      Los Angeles   
420         454 Main St, Seattle, WA 98101          Seattle   

      Quantidade(pedidos)  Total(valor_produto)  Valor(produto)  \
7043                    1                300.00         99.0000   
424                     1                109.99         71.4935   
423                     1                 14.95          7.4750   
3945                    1                999.99        329.9967   
420                     1                  2.99          1.4950   

      Turnover(ativos)       Data  Mês  Semana Nome do Mês Dia da Semana  \
7043            300.00 2019-01-01    1       1     Janeiro       Tuesday   
424             109.99 2019-01-01    1       1     Janeiro       Tuesday   
423              14.95 2019-01-01    1       1     Janeiro       Tuesday   
3945            999.99 2019-01-01    1       1     Janeiro       Tuesday   
420               2.99 2019-01-01    1       1     Janeiro       Tuesday   

     Dia da Semana Traduzido  Year        Mês/Year   Quarters  
7043             Terça-feira  2019  Janeiro - 2019  Quarter_1  
424              Terça-feira  2019  Janeiro - 2019  Quarter_1  
423              Terça-feira  2019  Janeiro - 2019  Quarter_1  
3945             Terça-feira  2019  Janeiro - 2019  Quarter_1  
420              Terça-feira  2019  Janeiro - 2019  Quarter_1  



Esse é o resultado da preparação e tratamento feito para análises posteriores: 
- Não foi visto valores nulos no dataframe 
- Não foi visto duplicatas no dataframe 
- A classificação das colunas estão ideais 
- Foi realizado uma formatação de tipo DATA 
- Foi Agrupado em Mês 
- Foi Agrupado em Semana 
- Foi passado o mês para extenso 
- Foi separado por Dia 
- Foi separado por Quarters 
- Foi separado em Mês + Ano 
- Foi tratado a coluna de endereços por cidade 


- Arquivo de: exploração_de_dados_sales_df 

