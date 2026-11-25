# Medidas DAX

## 1. Visão geral

As medidas DAX foram desenvolvidas para o acompanhamento dos resultados microbiológicos, identificação de não conformidades, análise temporal e integração dos indicadores com o mapeamento espacial da unidade industrial.

As medidas encontram-se organizadas em uma tabela específica, facilitando sua localização, organização e manutenção.

## 2. Indicadores de conformidade

| Medida | Finalidade |
|---|---|
| Qtd Conforme | Quantificação dos registros conformes. |
| Qtd Não Conforme | Quantificação dos registros não conformes. |
| Qtd NC Ano | Acompanhamento anual das não conformidades. |

## 3. Indicadores de mapeamento espacial

| Medida | Finalidade |
|---|---|
| Qtd NC MAPA | Quantificação das não conformidades para integração com o Synoptic Panel. |

A medida `Qtd NC MAPA` foi desenvolvida especificamente para alimentar a representação gráfica dos pontos de coleta na planta industrial.

Essa integração permite contextualizar espacialmente os resultados microbiológicos, facilitando a identificação dos pontos que apresentam não conformidades.

## 4. Classificação e formatação condicional

| Medida | Finalidade |
|---|---|
| Cor NC Ano | Classificação visual dos pontos conforme a quantidade anual de não conformidades. |
| Status Análise | Identificação do status das análises microbiológicas. |
| Status NC | Identificação do status relacionado às não conformidades. |

## 5. Controle temporal e acompanhamento

| Medida | Finalidade |
|---|---|
| Última Análise | Identificação da análise mais recente. |
| Última Coleta | Identificação da coleta mais recente. |
| Último Status | Identificação da condição de conformidade da última análise realizada no ponto. |

Esses indicadores auxiliam no acompanhamento histórico e na identificação da condição microbiológica mais recente dos pontos de monitoramento.

## 6. Aplicação das medidas

As medidas DAX complementam a estrutura dimensional e o mapeamento espacial, permitindo a análise das informações conforme os contextos de filtros estabelecidos no relatório.

Entre suas principais aplicações estão:

- Acompanhamento de conformidades e não conformidades.
- Análise histórica dos resultados microbiológicos.
- Identificação das últimas análises e coletas realizadas.
- Identificação do último status microbiológico.
- Representação visual de indicadores.
- Integração entre resultados laboratoriais e pontos de coleta.
- Contextualização dos indicadores conforme a localização selecionada.
- Identificação de pontos com histórico de reincidência.

## 7. Classificação visual de não conformidades

A medida `Cor NC Ano` foi desenvolvida para aplicação de formatação condicional baseada na quantidade acumulada de não conformidades por ponto de coleta durante o ano.

### Critérios de formatação condicional

| Quantidade anual de NC | Cor aplicada |
|---|---|
| 0 | 🟢 Verde |
| 1 a 2 | 🟡 Amarelo |
| 3 a 5 | 🟠 Laranja |
| 6 a 8 | 🔴 Vermelho |
| 9 ou mais | 🟣 Roxo |

Essa classificação permite identificar visualmente os pontos com maior quantidade acumulada de não conformidades, independentemente do resultado da última análise.

### Histórico microbiológico e condição atual

A utilização conjunta das medidas permite trabalhar com diferentes perspectivas analíticas:

- `Qtd NC Ano`: quantidade acumulada de não conformidades durante o ano.
- `Cor NC Ano`: representação visual do histórico de não conformidades.
- `Qtd NC MAPA`: integração das não conformidades com o mapeamento espacial.
- `Último Status`: identificação da condição microbiológica mais recente do ponto.

Dessa forma, um ponto pode apresentar conformidade na última análise e, simultaneamente, possuir uma classificação visual correspondente a um histórico elevado de não conformidades.

Essa distinção contribui para a investigação de recorrências e para a identificação de pontos que necessitam de maior atenção.

## 8. Possíveis melhorias futuras

- Desenvolvimento de indicadores de reincidência por ponto.
- Monitoramento do intervalo entre coletas.
- Identificação de pontos sem registros recentes.
- Indicadores de cumprimento da frequência de monitoramento.
- Identificação de tendências de não conformidade.
- Validação automatizada da correspondência entre pontos e resultados.
- Desenvolvimento de alertas para pontos com elevada quantidade de não conformidades.

## 9. Confidencialidade

A documentação apresenta a estrutura funcional das medidas DAX e os critérios de representação visual, sem divulgar resultados microbiológicos ou informações operacionais confidenciais.
