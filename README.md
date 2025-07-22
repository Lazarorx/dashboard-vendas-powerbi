Dashboard de Vendas – Power BI

Versão: 1.0  
Responsável Técnico: Lázaro Rafael Xavier  
Solicitante: UdiTech  
Data de Entrega: 22/07/2025  


Objetivo

Este projeto tem como objetivo o desenvolvimento de um dashboard interativo em Power BI para acompanhamento de vendas e indicadores operacionais de uma empresa de varejo. A ferramenta visa oferecer visibilidade estratégica ao time comercial, facilitando análises comparativas e tomadas de decisão baseadas em dados.


Arquivo do Projeto

Arquivo principal: `Projeto_final_lázaro.pbix`
Ferramenta: Power BI Desktop
Versão recomendada:** Julho/2025 (ou mais recente)



Escopo do Projeto

Visualizações e Indicadores:

- KPIs principais:  
  - Faturamento  
  - Quantidade de itens vendidos  
  - CMV  
  - Lucro Bruto  
  - Margem Bruta (%)

- Análises comparativas:  
  - MOM (Month over Month)  
  - LM (Último mês)  
  - YOY (Year over Year)  
  - LY (Ano anterior)

- Segmentações:  
  - Data  
  - Estado e cidade  
  - Vendedor  
  - Produto


Funcionalidades Implementadas

| Código | Requisito |

| RF01 | Filtros interativos sem necessidade de uso da tecla CTRL |
| RF02 | Tratamento de erros e vazios nas fórmulas de inteligência de tempo |
| RF03 | Gráfico de linha com evolução mensal de faturamento e quantidade |
| RF04 | Tabelas com top 3 produtos e clientes por faturamento |
| RF05 | Mapa com distribuição de margem por cidade |
| RF06 | TreeMap com % de margem por produto |


Fonte de Dados

- Origem: Planilha Excel local  
- Período: Dados de vendas 2024 e 2025  
- Tipo: Arquivo compartilhado (.xlsx)

Métricas Calculadas

| Indicador | Fórmula |

| Faturamento | `SUM(Valor de Venda)` |
| Quantidade | `SUM(Qtd)` |
| CMV | `SUM(CMV)` |
| Lucro Bruto | `[Faturamento] - [CMV]` |
| Margem Bruta % | `DIVIDE([Lucro Bruto], [Faturamento], 0)` |
| LM (Último Mês) | `PREVIOUSMONTH(dCalendario[Data])` |
| MOM | `DIVIDE([Faturamento], [LM], 0) - 1` |
| LY (Ano anterior) | `SAMEPERIODLASTYEAR(dCalendario[Data])` |
| YOY | `DIVIDE([Faturamento], [LY], 0) - 1` |



Estrutura do Dashboard

 Página 1 – Visão Geral:
- KPIs principais
- Filtros laterais
- Gráfico de evolução mensal
- Ranking de clientes e produtos
- Mapa com margem bruta por cidade

 Página 2 – Análise Detalhada:
- Filtros laterais
- Matriz com:
  - Linhas: Unidade, Vendedor
  - Colunas: Quantidade, Lucro Bruto, Faturamento, LM, LY



Cronograma do Projeto

| Etapa | Data | Responsável |

| Levantamento de Requisitos | 18/07 | BI + Solicitante |
| Modelagem dos Dados | 18/07 | Equipe de BI |
| Criação do Dashboard | 21/07 | BI |
| Validação | 22/07 | Solicitante |
| Publicação | 22/07 | BI |



Status

>  Projeto finalizado e validado pelo solicitante.
