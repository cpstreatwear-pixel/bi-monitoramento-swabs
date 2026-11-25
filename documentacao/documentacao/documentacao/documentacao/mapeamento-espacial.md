# Mapeamento Espacial e Integração com Synoptic Panel

## 1. Visão geral

O mapeamento espacial foi desenvolvido com o objetivo de integrar os resultados do monitoramento microbiológico à localização física dos pontos de coleta da unidade industrial.

O desenvolvimento envolveu a manipulação de plantas técnicas, conversão de arquivos, tratamento de imagens, desenvolvimento gráfico no Figma, edição da estrutura do código SVG e integração dos elementos interativos ao modelo de dados do Power BI.

## 2. Tecnologias e ferramentas utilizadas

| Ferramenta ou tecnologia | Aplicação |
|---|---|
| ZWCAD | Manipulação e adequação de plantas técnicas industriais. |
| Autodesk DWG TrueView | Visualização e preparação de arquivos DWG. |
| PDF | Formato intermediário de exportação das plantas. |
| JPG | Formato utilizado durante o tratamento das imagens. |
| Figma | Preparação gráfica, inclusão dos pontos de coleta e exportação dos arquivos SVG. |
| SVG | Representação gráfica dos mapas interativos. |
| XML | Manipulação do código e dos identificadores dos elementos SVG. |
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

### Fluxo de desenvolvimento

DWG → PDF → JPG → Figma → SVG → Edição do código SVG → Synoptic Panel → Power BI

A conversão e o tratamento das representações gráficas possibilitaram a construção de mapas personalizados para cada setor da unidade industrial.

## 5. Desenvolvimento gráfico no Figma

O Figma foi utilizado como ferramenta de preparação das representações gráficas e estruturação dos pontos de coleta.

As atividades contemplaram:

- Importação das imagens das plantas industriais.
- Organização das representações gráficas.
- Inclusão dos elementos representativos dos pontos de coleta.
- Posicionamento dos pontos conforme sua localização física.
- Organização dos elementos gráficos.
- Exportação dos arquivos no formato SVG.

A utilização do Figma permitiu personalizar a estrutura visual das plantas conforme as necessidades do projeto.

## 6. Manipulação do código SVG

Após a exportação dos arquivos pelo Figma, foi realizada a edição manual da estrutura do código SVG.

O formato SVG utiliza uma estrutura baseada em XML, permitindo a identificação e configuração individual dos elementos gráficos.

A manipulação do código teve como objetivo tornar os pontos de coleta elementos interativos, reconhecíveis pelo Synoptic Panel.

O processo contemplou:

- Edição da estrutura do código SVG.
- Identificação individual dos elementos gráficos.
- Adequação dos identificadores dos pontos de coleta.
- Associação dos elementos gráficos aos identificadores presentes no modelo de dados.
- Preparação dos elementos para seleção interativa.
- Compatibilização dos arquivos com o Synoptic Panel.

Essa etapa possibilitou transformar uma representação gráfica estática em uma interface interativa de análise de dados.

## 7. Levantamento e identificação dos pontos

O desenvolvimento contemplou a identificação dos pontos de monitoramento microbiológico e sua associação à localização física na planta industrial.

Foram consideradas as seguintes informações:

- Número de identificação do ponto.
- Setor de localização.
- Equipamento ou superfície monitorada.
- Associação com os processos produtivos.
- Correspondência com o cadastro geral de monitoramento.

Também foram consideradas situações em que um mesmo equipamento está associado a diferentes produtos ou processos, preservando a identificação única do ponto de coleta.

O levantamento contemplou ainda a identificação de necessidades de atualização das plantas técnicas.

## 8. Integração com o modelo dimensional

A dimensão de mapeamento geral concentra os identificadores únicos dos pontos de coleta da unidade.

Foram desenvolvidas tabelas auxiliares específicas para alimentar o Synoptic Panel de cada página setorial.

A integração estabelece a correspondência entre:

- Identificador do elemento SVG.
- Número do ponto de coleta.
- Cadastro geral de mapeamento.
- Tabela auxiliar setorial.
- Registros microbiológicos.

Essa arquitetura permite individualizar as representações gráficas dos setores sem perder a integração com a tabela central de resultados microbiológicos.

## 9. Interatividade

A integração entre o Synoptic Panel, os arquivos SVG personalizados e o modelo dimensional permite a análise dos resultados conforme a localização dos pontos de coleta.

Entre as funcionalidades desenvolvidas estão:

- Seleção interativa dos pontos representados na planta.
- Contextualização dos indicadores conforme a seleção.
- Análise dos resultados microbiológicos por localização.
- Identificação de não conformidades.
- Consulta da condição microbiológica mais recente.
- Acompanhamento das ocorrências acumuladas durante o ano.

## 10. Formatação condicional

Os pontos de coleta possuem representação visual associada à quantidade acumulada de não conformidades durante o ano.

| Quantidade anual de NC | Cor |
|---|---|
| 0 | 🟢 Verde |
| 1 a 2 | 🟡 Amarelo |
| 3 a 5 | 🟠 Laranja |
| 6 a 8 | 🔴 Vermelho |
| 9 ou mais | 🟣 Roxo |

A classificação permite identificar visualmente a concentração de ocorrências microbiológicas na unidade industrial.

O histórico acumulado de não conformidades é analisado separadamente da condição microbiológica mais recente do ponto.

## 11. Desafios técnicos

O desenvolvimento envolveu desafios relacionados à integração de diferentes estruturas de informação:

- Manipulação de arquivos de desenho técnico.
- Conversão entre diferentes formatos de arquivo.
- Tratamento e adequação das plantas industriais.
- Desenvolvimento de representações gráficas personalizadas no Figma.
- Manipulação manual da estrutura do código SVG.
- Transformação de elementos gráficos estáticos em elementos interativos.
- Compatibilização dos identificadores gráficos com as bases de dados.
- Representação de equipamentos associados a múltiplos processos.
- Organização das plantas e tabelas auxiliares por setor.
- Manutenção da correspondência entre a infraestrutura representada e o cadastro de monitoramento.

## 12. Possíveis melhorias futuras

- Versionamento das plantas utilizadas no relatório.
- Controle de alterações na localização dos pontos de coleta.
- Automatização da edição dos identificadores SVG.
- Validação automatizada da estrutura XML dos arquivos.
- Identificação de pontos cadastrados sem representação gráfica.
- Identificação de elementos gráficos sem correspondência na base de dados.
- Padronização do processo de atualização das plantas industriais.

## 13. Confidencialidade

As plantas técnicas originais, a localização dos equipamentos, a distribuição física dos pontos de coleta e os resultados microbiológicos constituem informações cuja divulgação depende de autorização.

A apresentação pública do projeto deverá utilizar representações gráficas demonstrativas, sem exposição da infraestrutura industrial real.


