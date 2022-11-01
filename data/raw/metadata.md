# Metadata

**daily_calendar_with_events.csv**

| Nome da Coluna | Tabela | Descrição |
| --- | --- | --- |
| date | calendar | data no formato y-m-d |
| weekday | calendar | dia da semana |
| weekday_int | calendar | dia numérico da semana (sábado dia 1, sexta-feira dia 7) |
| d | calendar | identificador de dia |
| event | calendar | se a data incluir um evento, o nome deste evento (apenas alguns estão incluídos) |

**item_prices.csv**

| Nome da Coluna | Tabela | Descrição |
| --- | --- | --- |
| item | prices | ID do produto |
| category | prices | Categoria de Produto |
| store_code | prices | Código alfanumérico da loja |
| yearweek | prices | Período de data para o preço (formato ano-semana) |
| sell_price | prices | Preço do produto “item” para o período em “anosemana”. Os preços são fornecidos por semana (média de 7 dias). Se não estiver disponível, não houve vendas para o produto
durante essa semana |

**item_sales.csv**

| Nome da Coluna | Tabela | Descrição |
| --- | --- | --- |
| id | sales | ID da série de vendas (combinação de item + store_code) |
| item | sales | ID do produto |
| category | sales | Categoria de produto |
| department | sales | ID do departamento (identificador diferente para lojas diferentes) |
| store | sales | Nome da loja |
| store_code | sales | ID da loja |
| region | sales | Região |
| d_1,d_2,d_… | sales | Número de unidades vendidas por dia |