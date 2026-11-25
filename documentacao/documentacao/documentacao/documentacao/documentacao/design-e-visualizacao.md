# Design e Visualização

## 1. Visão geral

O design do BI de Monitoramento Microbiológico de Swabs foi desenvolvido com foco na integração entre informações analíticas, navegação interativa e representações espaciais da unidade industrial.

O relatório permite acompanhar os resultados microbiológicos em diferentes níveis de detalhamento, desde uma visão consolidada da unidade até a análise individual dos pontos de coleta.

A estrutura visual foi desenvolvida para facilitar a identificação de não conformidades, a localização física das ocorrências e a consulta dos resultados microbiológicos.

## 2. Desenvolvimento da identidade visual

O layout do dashboard foi desenvolvido diretamente no Power BI Desktop, utilizando os recursos nativos de formatação e organização dos elementos visuais.

A estrutura contempla:

- Padronização dos cabeçalhos.
- Identidade visual institucional.
- Padronização das páginas setoriais.
- Organização dos elementos analíticos.
- Navegação interativa.
- Utilização de cores para identificação de ocorrências.
- Distribuição dos elementos conforme sua finalidade analítica.

O Figma foi utilizado especificamente na preparação das representações gráficas das plantas industriais, na inclusão dos pontos de coleta e na exportação dos arquivos SVG, posteriormente modificados para integração com o Synoptic Panel.

## 3. Arquitetura das páginas

O relatório está organizado em três níveis de visualização:

| Nível | Finalidade |
|---|---|
| Página inicial | Navegação espacial entre os setores industriais. |
| Visão geral | Análise consolidada e distribuição das não conformidades. |
| Páginas setoriais | Detalhamento espacial e analítico dos pontos de coleta. |

Essa organização permite que o usuário realize análises consolidadas ou direcionadas a determinados setores e pontos de monitoramento.

## 4. Página inicial — Navegação espacial

A página inicial apresenta uma representação geral da planta industrial, utilizada como interface de navegação entre os setores.

Os elementos gráficos foram configurados para permitir a interação com as áreas representadas, direcionando o usuário às respectivas páginas de detalhamento.

A página contempla:

- Representação geral da planta industrial.
- Identificação dos setores.
- Áreas gráficas interativas.
- Recursos de navegação entre páginas.
- Indicadores visuais.
- Legenda de classificação das não conformidades.
- Acesso a representações complementares de sistemas industriais.

A utilização da planta como interface de navegação permite substituir a dependência exclusiva de menus convencionais por uma experiência contextualizada à localização física dos setores.

## 5. Página de visão geral

A página de visão geral apresenta a consolidação das ocorrências microbiológicas da unidade industrial, permitindo a análise comparativa dos pontos de coleta e dos tipos de análises realizadas.

O layout foi organizado em duas áreas analíticas:

- Área superior: gráficos comparativos de não conformidades, distribuídos horizontalmente.
- Área inferior: gráfico de distribuição das não conformidades entre os pontos de coleta, denominado Análise de Tendência.

### 5.1. Indicadores apresentados

- Quantidade de não conformidades por ponto.
- Quantidade de não conformidades por tipo de análise microbiológica.
- Distribuição das não conformidades entre os pontos de monitoramento.
- Identificação dos pontos com maior concentração de ocorrências.

Os gráficos de barras horizontais permitem comparar as categorias e identificar aquelas com maior quantidade de não conformidades.

### 5.2. Segmentações de dados

A página contempla três segmentações:

| Segmentação | Finalidade |
|---|---|
| Mês | Delimitação do período de análise. |
| Número do ponto | Consulta direcionada pelo identificador do ponto de coleta. |
| Descrição do ponto | Consulta direcionada pela descrição do equipamento, superfície ou local monitorado. |

Esses recursos permitem realizar análises específicas sem a necessidade de navegar individualmente pelas páginas setoriais.

### 5.3. Análise de Tendência

Foi desenvolvido um gráfico de linhas, denominado Análise de Tendência, para representar a distribuição das não conformidades entre os pontos de coleta.

O visual utiliza os identificadores dos pontos no eixo horizontal e a quantidade de não conformidades no eixo vertical.

Sua aplicação permite:

- Identificar pontos com maior quantidade de ocorrências.
- Visualizar a concentração das não conformidades.
- Comparar a quantidade de ocorrências entre os pontos.
- Identificar pontos sem registros de não conformidades no contexto analisado.
- Avaliar a distribuição das ocorrências conforme os filtros aplicados.

Embora denominado Análise de Tendência no relatório, o gráfico representa uma distribuição por pontos de coleta, e não uma série temporal.

A utilização conjunta dos gráficos comparativos, das segmentações e da análise de distribuição permite aprofundar a avaliação consolidada dos resultados microbiológicos.

## 6. Páginas de detalhamento setorial

As páginas setoriais apresentam informações específicas dos respectivos ambientes industriais.

Cada página integra a representação espacial dos pontos de coleta aos indicadores microbiológicos correspondentes.

### 6.1. Organização do layout

| Área | Finalidade |
|---|---|
| Cabeçalho | Identidade visual, navegação e segmentação temporal. |
| Área esquerda | Planta industrial interativa com os pontos de coleta. |
| Área superior direita | Tabela de registros microbiológicos. |
| Área central direita | Quantidade de não conformidades por ponto. |
| Área inferior direita | Quantidade de não conformidades por mês. |

A distribuição dos elementos permite relacionar a localização física dos pontos com os resultados apresentados nos indicadores.

## 7. Elementos visuais

### 7.1. Synoptic Panel

Visual personalizado utilizado para representar os setores e pontos de monitoramento sobre as plantas industriais.

A integração com arquivos SVG personalizados permite a identificação individual dos elementos gráficos e sua associação ao modelo de dados.

O visual possibilita:

- Identificação espacial dos pontos.
- Aplicação de formatação condicional.
- Seleção individual dos pontos de coleta.
- Interação com os demais elementos analíticos.
- Apresentação de tooltips personalizados.
- Consulta de informações microbiológicas contextualizadas.

### 7.2. Tabela de registros microbiológicos

Visual destinado ao detalhamento das ocorrências microbiológicas.

A tabela apresenta informações como:

- Data.
- Descrição do ponto.
- Tipo de análise.
- Resultado de conformidade ou não conformidade.
- Número da R.A., quando aplicável.

### 7.3. Gráficos de barras horizontais

Utilizados na página de visão geral para comparação das quantidades de não conformidades entre pontos e tipos de análises microbiológicas.

A organização dos valores permite identificar as categorias com maior quantidade de ocorrências.

### 7.4. Gráfico de não conformidades por ponto

Gráfico de linhas utilizado nas páginas setoriais para apresentar a quantidade de ocorrências associadas aos pontos de monitoramento.

### 7.5. Gráfico de não conformidades por mês

Gráfico de linhas destinado ao acompanhamento da distribuição temporal das ocorrências microbiológicas.

Permite identificar os períodos com maior quantidade de não conformidades.

### 7.6. Gráfico de análise de distribuição

Gráfico de linhas utilizado na página de visão geral, denominado Análise de Tendência, destinado à representação da distribuição das não conformidades entre os identificadores dos pontos de coleta.

O visual complementa os gráficos comparativos e permite avaliar a concentração das ocorrências microbiológicas.

### 7.7. Segmentações de dados

As segmentações permitem contextualizar os indicadores conforme o período e os pontos de monitoramento selecionados.

Nas páginas setoriais, é utilizada a segmentação por mês.

Na página de visão geral, são utilizadas segmentações por mês, número do ponto e descrição do ponto.

## 8. Navegação e interatividade

O relatório utiliza recursos de navegação entre páginas, drill-through e interação entre elementos visuais.

A estrutura de navegação contempla:

- Seleção dos setores na planta geral.
- Acesso às páginas de detalhamento setorial.
- Seleção individual dos pontos de coleta.
- Consulta dos indicadores associados à localização selecionada.
- Navegação de retorno.
- Consulta da visão consolidada das não conformidades.
- Aplicação de filtros direcionados aos pontos de coleta.
- Consulta rápida de informações por meio de tooltips.

A integração entre os arquivos SVG, o Synoptic Panel e o modelo dimensional permite utilizar a representação física da unidade como parte da interface analítica.

## 9. Tooltips personalizados

Foram desenvolvidas páginas personalizadas de dicas de ferramentas (tooltips), integradas aos elementos gráficos do Synoptic Panel.

Ao posicionar o cursor sobre um ponto de coleta representado na planta industrial, o relatório apresenta automaticamente informações relacionadas ao respectivo ponto, sem necessidade de selecioná-lo ou navegar para outra página.

### 9.1. Informações apresentadas

O tooltip contempla dois elementos visuais.

**Tabela de detalhamento microbiológico:**

- Tipo de análise microbiológica.
- Quantidade de resultados não conformes.
- Data da ocorrência.
- Total de não conformidades.

**Gráfico de distribuição temporal:**

- Quantidade de não conformidades por mês.
- Utilização da medida DAX `Qtd NC MAPA`.
- Contextualização dos resultados conforme o ponto sobre o qual o cursor está posicionado.

### 9.2. Contexto de filtragem

As informações apresentadas no tooltip são contextualizadas pelo ponto de coleta, utilizando a integração entre o Synoptic Panel e o modelo dimensional.

Essa estrutura permite apresentar informações específicas de cada ponto, evitando a necessidade de disponibilizar todos os detalhes simultaneamente na página principal.

### 9.3. Benefícios da implementação

- Consulta rápida das ocorrências microbiológicas.
- Identificação dos tipos de análises não conformes.
- Visualização das datas das ocorrências.
- Acompanhamento da distribuição temporal.
- Redução da necessidade de navegação entre páginas.
- Preservação da organização visual do relatório.
- Ampliação da interatividade das plantas industriais.

A utilização dos tooltips permite transformar os pontos de coleta em elementos de consulta dinâmica, complementando a classificação visual das não conformidades apresentada na planta.

## 10. Formatação condicional

A representação gráfica dos pontos de coleta utiliza uma escala de cores baseada na quantidade acumulada de não conformidades durante o ano.

| Quantidade anual de NC | Representação visual |
|---|---|
| 0 | 🟢 Verde |
| 1 a 2 | 🟡 Amarelo |
| 3 a 5 | 🟠 Laranja |
| 6 a 8 | 🔴 Vermelho |
| 9 ou mais | 🟣 Roxo |

A classificação permite identificar pontos com maior quantidade de ocorrências microbiológicas, direcionando a atenção do usuário durante a análise espacial.

O histórico acumulado de não conformidades é analisado separadamente da condição microbiológica mais recente do ponto.

A classificação representa a quantidade de ocorrências registradas, não necessariamente a gravidade microbiológica de cada resultado.

## 11. Níveis de interação

A experiência do usuário pode ser organizada conceitualmente em quatro níveis de interação.

| Nível | Interação | Finalidade |
|---|---|---|
| 1 | Navegação espacial | Acesso às páginas setoriais por meio da planta geral. |
| 2 | Identificação visual | Identificação da quantidade acumulada de não conformidades pela cor dos pontos. |
| 3 | Consulta rápida | Apresentação de informações complementares ao posicionar o cursor sobre o ponto. |
| 4 | Detalhamento analítico | Seleção do ponto e consulta dos indicadores associados. |

Essa estrutura permite diferentes níveis de aprofundamento das informações, conforme a necessidade do usuário.

## 12. Experiência do usuário

O desenvolvimento visual foi direcionado à simplificação da consulta dos resultados microbiológicos.

A arquitetura do relatório permite diferentes abordagens de análise:

- Análise consolidada da unidade.
- Navegação espacial entre setores.
- Localização física dos pontos de coleta.
- Análise individual dos pontos.
- Comparação das ocorrências entre pontos.
- Comparação entre tipos de análises microbiológicas.
- Acompanhamento temporal das não conformidades.
- Análise da concentração das ocorrências.
- Consulta direcionada pelo número ou descrição do ponto.
- Consulta de registros detalhados.
- Consulta dinâmica de informações por meio de tooltips.

A integração entre elementos gráficos e informações analíticas permite reduzir a dependência de consultas manuais às bases de dados.

## 13. Diferenciais do projeto

- Utilização da planta industrial como interface de navegação.
- Integração entre desenho técnico, design gráfico e Business Intelligence.
- Desenvolvimento de representações gráficas no Figma.
- Desenvolvimento de arquivos SVG personalizados.
- Manipulação manual da estrutura XML dos arquivos gráficos.
- Configuração de elementos gráficos interativos.
- Navegação espacial em diferentes níveis de detalhamento.
- Associação entre localização física e resultados microbiológicos.
- Classificação visual das ocorrências por formatação condicional.
- Integração entre indicadores consolidados e análises setoriais.
- Análise da distribuição e concentração das não conformidades.
- Segmentações direcionadas à identificação dos pontos de coleta.
- Desenvolvimento de tooltips contextualizados por ponto de coleta.
- Utilização de recursos de navegação interativa e drill-through.

## 14. Possíveis melhorias futuras

### 14.1. Melhorias visuais

- Aprimoramento da acessibilidade visual.
- Utilização de elementos complementares às cores para identificação das classificações.
- Aprimoramento da ordenação cronológica dos indicadores.
- Tratamento de categorias temporais sem identificação.
- Padronização dos títulos dos elementos visuais.
- Avaliação de gráficos de barras para comparação entre pontos nas páginas setoriais.
- Padronização dos tooltips entre as páginas.
- Validação da correspondência entre as legendas e as medidas de formatação condicional.

### 14.2. Evolução dos indicadores analíticos

- Desenvolvimento de gráficos de Pareto para identificação dos pontos responsáveis pela maior concentração de não conformidades.
- Desenvolvimento de indicadores de taxa de não conformidade em relação à quantidade total de análises.
- Desenvolvimento de indicadores de cumprimento das frequências de coleta.
- Implementação de análises de tendência temporal.
- Desenvolvimento de indicadores de reincidência microbiológica.
- Comparação proporcional entre pontos com diferentes frequências de monitoramento.

A utilização de indicadores proporcionais poderá complementar a análise das quantidades absolutas de não conformidades, considerando que os pontos possuem diferentes frequências de coleta.

### 14.3. Apresentação demonstrativa

- Desenvolvimento de uma versão demonstrativa com dados fictícios.
- Criação de plantas industriais ilustrativas.
- Preservação das funcionalidades de navegação e interatividade.
- Demonstração da integração entre arquivos SVG e o modelo dimensional.

## 15. Confidencialidade

A identidade visual institucional, as plantas industriais, os registros microbiológicos e as informações operacionais não serão disponibilizados publicamente sem autorização.

As representações utilizadas para apresentação do projeto em portfólio deverão preservar os conceitos técnicos e visuais desenvolvidos, utilizando informações e estruturas gráficas fictícias.

A documentação tem como finalidade demonstrar as competências técnicas aplicadas durante o desenvolvimento do projeto, sem comprometer a confidencialidade das informações corporativas.
