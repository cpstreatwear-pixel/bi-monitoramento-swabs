# Mapeamento Espacial e Integração com Synoptic Panel

## 1. Visão geral

O mapeamento espacial foi desenvolvido com o objetivo de integrar os resultados do monitoramento microbiológico à localização física dos pontos de coleta da unidade industrial.

O desenvolvimento envolveu a manipulação de plantas técnicas, conversão de arquivos, tratamento de imagens, identificação de pontos de coleta e integração das representações gráficas ao modelo de dados do Power BI.

## 2. Tecnologias e ferramentas utilizadas

| Ferramenta | Aplicação |
|---|---|
| ZWCAD | Manipulação e adequação de plantas técnicas industriais. |
| Autodesk DWG TrueView | Visualização e preparação de arquivos DWG. |
| PDF | Formato intermediário de exportação das plantas. |
| JPG | Formato utilizado durante o tratamento das imagens. |
| SVG | Formato utilizado para representação gráfica interativa. |
| Synoptic Panel by OKViz | Integração entre os elementos gráficos e o modelo de dados. |
| Power BI Desktop | Desenvolvimento do relatório e configuração das interações. |
| DAX | Desenvolvimento dos indicadores associados ao mapeamento. |

## 3. Preparação das plantas industriais

As plantas técnicas originais passaram por procedimentos de adequação para utilização no ambiente analítico.

O processo contemplou:

- Visualização e manipulação dos arquivos DWG.
- Separação das representações gráficas por setor.
- Adequação das áreas de interesse.
- Remoção de elementos gráficos desnecessários.
- Correção e tratamento das imagens.
- Preparação das plantas para identificação dos pontos de coleta.

Essas etapas permitiram adaptar uma representação originalmente destinada à visualização técnica da infraestrutura para uma aplicação de Business Intelligence.

## 4. Conversão dos arquivos

O processo de preparação gráfica utilizou diferentes formatos de arquivo até a obtenção da estrutura compatível com o Synoptic Panel.

### Fluxo de conversão

DWG → PDF → JPG → SVG → Synoptic Panel → Power BI

A utilização do formato SVG possibilitou a identificação individual dos elementos gráficos associados aos pontos de coleta.

## 5. Levantamento e identificação dos pontos

O desenvolvimento contemplou a identificação dos pontos de monitoramento microbiológico e sua associação à localização física na planta industrial.

Foram consideradas as seguintes informações:

- Número de identificação do ponto.
- Setor de localização.
- Equipamento ou superfície monitorada.
- Associação com os processos produtivos.
- Correspondência com o cadastro geral de monitoramento.

Também foram consideradas situações em que um mesmo equipamento está associado a diferentes produtos ou processos, preservando a identificação única do ponto de coleta.

O levantamento contemplou ainda a identificação de necessidades de atualização das plantas técnicas.

## 6. Estruturação dos elementos gráficos

Após o tratamento das imagens, foram adicionados elementos gráficos representativos dos pontos de coleta.

Cada elemento foi associado ao identificador correspondente no modelo de dados.

Essa estrutura possibilita estabelecer uma correspondência entre:

- Elemento gráfico.
- Número do ponto.
- Cadastro geral de mapeamento.
- Tabela setorial.
- Registros microbiológicos.

## 7. Integração com o modelo dimensional

A dimensão de mapeamento geral concentra os identificadores únicos dos pontos de coleta da unidade.

Foram desenvolvidas tabelas auxiliares específicas para alimentar o Synoptic Panel de cada página setorial.

Essa arquitetura permite individualizar as representações gráficas dos setores sem perder a integração com a tabela central de resultados microbiológicos.

## 8. Interatividade

A integração entre o Synoptic Panel e o modelo dimensional permite a análise dos resultados conforme a localização dos pontos de coleta.

Entre as funcionalidades desenvolvidas estão:

- Seleção interativa dos pontos representados na planta.
- Contextualização dos indicadores conforme a seleção.
- Análise dos resultados microbiológicos por localização.
- Identificação de não conformidades.
- Consulta da condição microbiológica mais recente.
- Acompanhamento das ocorrências acumuladas durante o ano.

## 9. Formatação condicional

Os pontos de coleta possuem representação visual associada à quantidade acumulada de não conformidades durante o ano.

| Quantidade anual de NC | Cor |
|---|---|
| 0 | Verde |
| 1 a 2 | Amarelo |
| 3 a 5 | Laranja |
| 6 a 8 | Vermelho |
| 9 ou mais | Roxo |

A classificação permite identificar visualmente a concentração de ocorrências microbiológicas na unidade industrial.

O histórico acumulado de não conformidades é analisado separadamente da condição microbiológica mais recente do ponto.

## 10. Desafios técnicos

O desenvolvimento envolveu desafios relacionados à integração de diferentes estruturas de informação:

- Adequação de arquivos técnicos para utilização em ferramentas analíticas.
- Conversão entre diferentes formatos de arquivo.
- Identificação física e gráfica dos pontos de coleta.
- Compatibilização dos identificadores gráficos com as bases de dados.
- Representação de equipamentos associados a múltiplos processos.
- Organização das plantas e tabelas auxiliares por setor.
- Manutenção da correspondência entre a infraestrutura representada e o cadastro de monitoramento.

## 11. Possíveis melhorias futuras

- Versionamento das plantas utilizadas no relatório.
- Controle de alterações na localização dos pontos de coleta.
- Validação automatizada dos identificadores presentes nos arquivos SVG.
- Identificação de pontos cadastrados sem representação gráfica.
- Identificação de elementos gráficos sem correspondência na base de dados.
- Padronização do processo de atualização das plantas industriais.

## 12. Confidencialidade

As plantas técnicas originais, a localização dos equipamentos, a distribuição física dos pontos de coleta e os resultados microbiológicos constituem informações cuja divulgação depende de autorização.

A apresentação pública do projeto deverá utilizar representações gráficas demonstrativas, sem exposição da infraestrutura industrial real.
