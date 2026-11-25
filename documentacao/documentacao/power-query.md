# Power Query e Processos de ETL

## 1. Visão geral

O processo de ETL foi desenvolvido para garantir a preparação, organização e integração dos dados de monitoramento microbiológico ambiental ao modelo dimensional e às estruturas auxiliares de mapeamento espacial.

## 2. Extração de dados

A extração das informações é realizada por meio da conexão com bases de dados mantidas no Google Planilhas.

As informações são importadas para o Power BI, permitindo a aplicação de procedimentos de tratamento e transformação antes do carregamento no modelo.

## 3. Limpeza e tratamento dos dados

Foram aplicados os seguintes procedimentos:

- Alteração e adequação dos tipos de dados.
- Remoção de linhas desnecessárias.
- Remoção de colunas não utilizadas.
- Remoção de duplicidades.
- Tratamento de valores nulos.
- Tratamento de erros.
- Tratamento e adequação de campos de data.

Esses procedimentos contribuem para a consistência das informações e a redução de problemas durante o processamento dos dados.

## 4. Transformações e estruturas auxiliares

Durante o desenvolvimento, foram utilizadas colunas condicionais e tabelas auxiliares para complementar a estrutura analítica do projeto.

As tabelas auxiliares de mapeamento foram organizadas conforme os setores e equipamentos representados nas páginas do relatório.

Essa estrutura permite a integração dos registros microbiológicos ao cadastro centralizado dos pontos de coleta e aos respectivos mapas interativos.

## 5. Carregamento e integração

Após o tratamento, as informações são carregadas no modelo dimensional do Power BI.

A integração contempla:

- Tabela central de resultados microbiológicos.
- Dimensão de análises.
- Dimensão calendário.
- Dimensão de turnos.
- Cadastro geral dos pontos de coleta.
- Estruturas auxiliares de mapeamento setorial.

## 6. Atualização e manutenção

O projeto contempla procedimentos de manutenção das conexões e atualização das informações no Power BI Service.

Foram realizadas as seguintes atividades:

- Configuração de credenciais das fontes de dados.
- Configuração de atualização agendada.
- Identificação e correção de erros de atualização.

## 7. Integração com a estrutura gráfica

Além do tratamento das bases de dados, o projeto contempla um fluxo independente de preparação das plantas industriais.

A estrutura gráfica é associada ao modelo por meio dos identificadores dos pontos de coleta, permitindo a integração entre os resultados microbiológicos e sua localização física.

Os procedimentos de preparação gráfica e integração espacial são detalhados na documentação de mapeamento espacial.

## 8. Possíveis melhorias futuras

- Validação automatizada dos números dos pontos de coleta.
- Identificação de registros sem correspondência no cadastro geral.
- Monitoramento de inconsistências nas fontes de dados.
- Identificação de campos obrigatórios não preenchidos.
- Monitoramento automatizado de falhas de atualização.
- Validação da correspondência entre identificadores gráficos e registros microbiológicos.

## 9. Confidencialidade

A documentação descreve os procedimentos técnicos de tratamento e integração, sem disponibilizar bases corporativas ou informações operacionais confidenciais.
