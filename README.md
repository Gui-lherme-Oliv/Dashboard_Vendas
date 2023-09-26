# Criação de dashboard com dados de vendas utilizando Power BI
#### Autor: Guilherme Oliveira da Rocha Cunha

## 1. Dados
Os dados foram disponibilizados pela plataforma Udemy. Trata-se de uma tabela chamada "vendas" que simula as vendas de uma empresa em formato Excel (.xlsx), com 400 linhas e 7 colunas:
- **VendasID**: Identificador de cada venda
- **Vendedor**: Nome do vendedor de cada venda
- **Cliente**: Cliente de cada venda
- **Data**: Data de cada venda
- **Produto**: Produto que foi vendido
- **ValorUni**: Valor unitário do produto que foi vendido
- **Quantidade**: Quantidade de produto vendido em cada venda

## 2. Preparação
Em uma análise dos dados na tabela Excel foi visto que não existiam valores nulos ou duplicados. Então a tabela foi inserida no Power BI e realizado os seguintes procedimentos:
- A coluna **VendasID** foi ocultada pois não será necessária para o estudo
- O formato da coluna **Data** foi alterado para o padrão dd/mm/yyyy
- O formato da coluna **ValorUni** foi alterado para Moeda com 2 casas decimais
- Criada uma nova coluna chamada **Total**, onde nela foi utilizada a fórmula Total = Vendas[Quantidade] * Vendas[ValorUni], e alterado o formato para Moeda com 2 casas decimais. Essa coluna representa o valor total de cada venda.

## 3. Criação do painel Vendas
Foram inseridos os seguintes gráficos:
- **Total de vendas**: Gráfico de área com o eixo X sendo o campo **Data** e o eixo Y sendo o campo **Total** para mostrar o total de vendas de acordo com o tempo. Pode ser disposto por ano, trimestre, mês ou dia.
- **Total de vendas por produto**: Gráfico de colunas clusterizado com o eixo X sendo o campo **Data**, eixo Y sendo o campo **Total** e legenda sendo o campo **Produto** para mostrar o total de vendas de cada produto de acordo com o tempo. Pode ser disposto por ano, trimestre, mês ou dia.

## 4. Criação do painel Melhores
Foram inseridos os seguintes gráficos:
- **Melhores clientes**: Gráfico de pizza com a legenda sendo o campo **Cliente** e os valores o campo **Total** com o filtro N superior no campo **Cliente** definido para mostrar os 5 maiores compradores, ou seja, os 5 clientes que mais gastaram em compras.
- **Produtos mais vendidos**: Gráfico de colunas clusterizados com o eixo Y sendo o campo **Total** e a legenda sendo o campo **Produto** com o filtro N superior no campo **Produto** definido para mostrar os 5 produtos mais vendidos.
- **Vendedores que mais venderam**: Gráfico de colunas clusterizado com o eixo X sendo o campo **Vendedor** e o eixo Y sendo o campo **Total** com o filtro N superior no campo **Vendedor** definido para mostrar os 5 vendedores que mais venderam.
- **Vendedores que menos venderam**: Gráfico de colunas clusterizado com o eixo X sendo o campo **Vendedor** e o eixo Y sendo o campo **Total** com o filtro N superior no campo **Vendedor** definido para mostrar os 5 vendedores que menos venderam.
- **Tabelas**: Duas tabelas inseridas, uma apresentando os produtos disponíveis e outra apresentando os nomes dos vendedores.

## 5. Resultados
O arquivo manipulável para ser acessado através do Power BI contendo toda a análise pode ser obtido em AnaliseVendas.pbix, arquivo aqui disponiblizado.
### Painel Vendas
![Vendas](https://github.com/Gui-lherme-Oliv/Dashboard_Vendas/assets/123426025/ed3742cf-ec53-4a90-bfb4-0e01ad7e5a4c)
### Painel Melhores
![Melhores](https://github.com/Gui-lherme-Oliv/Dashboard_Vendas/assets/123426025/0be1b160-5f57-40ff-b0c6-d9bc9a7e9e34)














