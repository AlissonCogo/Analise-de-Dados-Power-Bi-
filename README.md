# Portfólio Power BI 📊

Dashboards elaborados com foco em estudos na ferramenta Power BI

Acessando [Aqui](https://app.powerbi.com/view?r=eyJrIjoiZjM5NzljMjctZjU1ZC00YTMyLThlODItZTI0NDhjNGNjYTk1IiwidCI6IjMxYmM0MmM1LTIwMzAtNDVkNC1hYzBlLWYxZDY4M2VmYjZlZiJ9
), voce tem o acesso ao dashboard do PetShop Gatito aonde traz algumas informações sobre a análise dos dados entre o período de 12/2020 a 12/2022 possibilitando o manuseamento dos dados.

O DashBoard Possui Filtros de Ano, Produtos e Marca(Cachorro, gatito)!

# Estrutura da base de dados

## Arquivo em Excel que contém inicialmente as seguintes colunas:

### Vendas:
- Data da Compras
- - ID Consumidor
- Id Produto
- Quantidade
- Transacao

#### Criado 2 nova **Coluna** a partir dos dados:
- Valor Unitário Produto (Valor Unitário Produto = RELATED(Produtos[Valor]))
- Faturamento Total (Faturamento Total = Vendas[Quantidade] * Vendas[Valor Unitário Produto])

### Produtos:
- Categoria
- ID Produto
- Marca
- Nome Produto
- Url img
- Valor

#### Criado 1 nova **Medida** a partir dos dados:
- Valor Médio Por Produto (Valor Médio Por Produto = SUM(Produtos[Valor]) / COUNT(Produtos[ID Produto]))


## Arquivo em Csv que contém inicialmente as seguintes colunas:

### Clientes:
- Bairro
- Estado Civil
- Gênero
- ID Consumidor
- Pets

#### Não foi Criado nenhuma Coluna/Medida a partir dos dados  



