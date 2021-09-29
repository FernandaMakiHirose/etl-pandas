# Fundamentos de ETL com Python
- Extract: os dados são extraídos de diferentes fontes de dados
- Transform: Propagados para a área de preparação de dados, onde são transformados e limpos
- Load: Carregados no data warehouse

## Requisitos
- [Anaconda](https://www.anaconda.com/products/individual)
- Jupyter Notebook e conhecimento na ferramenta
- Python
- Pandas

## Licença
Distribuido sob a licença MIT License. Veja `LICENSE` para mais informações

## Executar o projeto
Abra o projeto no Jupyter Notebook e execute o projeto clicando em `Run`

## Quiz
### Suponha que desejamos selecionar apenas as linhas de um dataframe "df" em que o valor da coluna "seminario" seja acima de 8.0 e o valor da coluna "prova" NÃO seja menor que 3. Identifique a instrução que contenha o filtro que permite realizar essa operação:
df.loc[(df["seminario"] > 8.0) & (df["prova"] >= 3)]

### No processo de extração de dados de um arquivo CSV utilizando a biblioteca Pandas por meio da função read_csv, é possível fazer a checagem dos dados do tipo data utilizando o parâmetro:
parse_dates

### Um Data Warehouse (DW) possui uma grande quantidade de dados advindos de outras fontes. Neste contexto, o processo de ETL:
Realiza a função de extração, possível limpeza e readequação dos dados para que estes possam ser carregados no DW

### Em um dataframe que possui 100 linhas, a função tail exibe por padrão:
As cinco últimas linhas do dataframe

### Quais dos valores abaixo NÃO é considerado, por padrão, um valor ausente pela função fillna da biblioteca pandas:
0

### Em processos ligados a ETL, os dados são identificados e extraídos de:
Diferentes fontes, como, por exemplo, arquivos CSV, banco de dados, entre outros

### Suponha que um dataframe "df" contenha a coluna "data" do tipo datetime64[ns] e a coluna "valor" do tipo float64. Qual instrução permite exibir a soma dos valores agrupados por ano e mês respectivamente:
df.groupby([df.data.dt.year,df.data.dt.month]).valor.sum()

### O seguinte trecho de código utiliza um filtro na coluna "ocorrencia_cidade" do dataframe "df". Para este filtro, é correto afirmar que:
```
filtro = df.ocorrencia_cidade.str[-1] == 'E'
df.loc[filtro]
```

Seleciona dados cuja cidade termina com a letra E
