# Criação de dashboard com dados de vendas utilizando Power BI
#### Autor: Guilherme Oliveira da Rocha Cunha

## 1. Dados
Os dados foram disponibilizados pela plataforma Udemy. Trata-se de uma tabela simulando as vendas de uma empresa em formato Excel (.xlsx), com 400 linhas e 7 colunas:
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
- Criada uma nova coluna chamada Total, onde nela foi utilizada a fórmula Total = Vendas[Quantidade] * Vendas[ValorUni], e alterei o formato para Moeda com 2 casas decimais. Essa coluna representa o valor total de cada venda.

## 3. Criação do painél Vendas
