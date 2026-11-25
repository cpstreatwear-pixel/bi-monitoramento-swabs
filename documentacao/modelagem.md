# Modelagem de Dados

## 1. Arquitetura do modelo

O projeto utiliza uma arquitetura dimensional com núcleo em estrela, complementada por estruturas auxiliares destinadas ao mapeamento espacial dos pontos de coleta microbiológica.

A modelagem foi desenvolvida considerando a necessidade de integrar resultados laboratoriais, informações temporais, turnos, tipos de análises e localização física dos pontos de monitoramento.

## 2. Tabela fato

A tabela central de resultados microbiológicos concentra os registros das análises realizadas e estabelece relacionamentos com as dimensões responsáveis pela contextualização das informações.

A estrutura permite a análise dos resultados considerando:

- Data de coleta.
- Tipo de análise microbiológica.
- Número do ponto de coleta.
- Turno.
- Localização do ponto.

## 3. Dimensões

### Mapeamento Geral

Dimensão central responsável pela identificação dos pontos de coleta e pela conexão entre os registros microbiológicos e as estruturas auxiliares de mapeamento setorial.

O número do ponto de coleta constitui a principal chave de relacionamento dessa estrutura.

### Dimensão de Análises

Responsável pela identificação dos tipos de análises microbiológicas, utilizando códigos de análise como referência de relacionamento.

### Dimensão Calendário

Responsável pela contextualização temporal dos registros, permitindo a aplicação de filtros e análises históricas.

### Dimensão Turno

Responsável pela segmentação das informações conforme os turnos operacionais.

## 4. Estruturas auxiliares de mapeamento

Foram desenvolvidas tabelas específicas para representar os diferentes setores, equipamentos e agrupamentos de pontos de coleta da unidade industrial.

Cada tabela setorial foi estruturada para alimentar o visual personalizado Synoptic Panel by OKViz da respectiva página do relatório.

A dimensão Mapeamento Geral concentra todos os pontos de coleta da unidade, utilizando identificadores únicos, sem duplicidade no número do ponto.

Essa arquitetura permite:

- Manter um cadastro centralizado dos pontos de coleta.
- Individualizar as representações gráficas de cada setor.
- Integrar os elementos espaciais aos resultados microbiológicos.
- Propagar filtros entre o mapeamento setorial e os registros analíticos.
- Preservar a identificação dos pontos independentemente da página de visualização.

## 5. Relacionamentos

O modelo contempla diferentes configurações de cardinalidade e propagação de filtros.

| Estrutura | Cardinalidade | Direção de filtro |
|---|---|---|
| Dimensões e tabela fato | 1:N | Unidirecional |
| Mapeamento geral e tabelas setoriais | 1:1 | Bidirecional |
| Cadastro auxiliar de localização e mapeamento | 1:N | Unidirecional |

A estrutura também contempla relacionamento auxiliar inativo entre tabelas de localização.

## 6. Integração com o mapeamento espacial

A identificação dos pontos de coleta permite estabelecer a correspondência entre os registros microbiológicos e os elementos gráficos utilizados na representação da planta industrial.

Essa integração possibilita a contextualização espacial dos resultados e complementa a análise convencional por indicadores, gráficos e filtros.

## 7. Particularidades da modelagem

- Integração de dados microbiológicos e informações espaciais.
- Utilização do número do ponto como referência central de identificação.
- Estruturas auxiliares específicas para diferentes setores.
- Relacionamentos bidirecionais nas estruturas de mapeamento.
- Separação entre registros analíticos e cadastros de identificação.
- Integração com visual personalizado do Power BI.

## 8. Possíveis melhorias futuras

- Implementação de validações automatizadas dos identificadores dos pontos.
- Identificação de registros sem correspondência no cadastro de mapeamento.
- Monitoramento da integridade referencial.
- Avaliação da necessidade dos relacionamentos bidirecionais.
- Controle de alterações e versionamento do cadastro de pontos de coleta.
- Documentação das dependências entre os elementos gráficos e os identificadores utilizados no modelo.

## 9. Confidencialidade

A documentação apresenta a arquitetura conceitual do projeto, preservando informações relacionadas à infraestrutura industrial, à localização específica dos pontos e aos resultados microbiológicos corporativos.
