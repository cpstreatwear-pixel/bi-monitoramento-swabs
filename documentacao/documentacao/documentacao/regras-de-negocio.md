# Regras de Negócio

## 1. Visão geral

O BI de Monitoramento Microbiológico de Swabs foi desenvolvido para acompanhar os resultados das análises microbiológicas realizadas nos pontos de coleta da unidade industrial, considerando suas particularidades operacionais, localização física e histórico de resultados.

## 2. Identificação dos pontos de coleta

Cada ponto de coleta possui um identificador único, registrado no cadastro de mapeamento geral.

Esse identificador permite estabelecer a correspondência entre:

- Localização física.
- Setor industrial.
- Equipamento ou superfície monitorada.
- Representação gráfica na planta industrial.
- Registros de análises microbiológicas.

Um mesmo ponto pode estar associado a diferentes produtos, processos e tipos de análises.

## 3. Frequência de monitoramento

Os pontos de coleta possuem diferentes frequências de monitoramento, conforme os critérios estabelecidos para cada local e processo.

Todos os pontos cadastrados devem ser contemplados pelo monitoramento microbiológico, respeitando suas respectivas frequências de coleta.

A ausência de registros deve ser analisada considerando a periodicidade aplicável ao ponto.

## 4. Tipos de análises microbiológicas

Um mesmo ponto de coleta pode receber diferentes tipos de análises microbiológicas.

A estrutura do modelo permite segmentar os resultados conforme o tipo de análise, preservando a identificação do ponto e seu contexto operacional.

## 5. Classificação dos resultados

A classificação dos resultados microbiológicos é realizada diretamente na fonte de dados.

O Power BI utiliza as classificações registradas na base para realizar a consolidação dos indicadores de conformidade e não conformidade.

O dashboard não substitui os critérios técnicos utilizados na avaliação laboratorial dos resultados.

## 6. Reverificação de não conformidades

Quando um resultado apresenta não conformidade, é realizada uma nova coleta para acompanhamento da condição microbiológica do ponto.

O dashboard contempla o acompanhamento dessas reverificações, permitindo consultar os resultados posteriores à identificação da não conformidade.

A conformidade de uma análise posterior não elimina o registro histórico da ocorrência anterior.

## 7. Monitoramento por turno

Um mesmo ponto de coleta pode ser monitorado em diferentes turnos operacionais.

A dimensão de turnos permite segmentar os resultados microbiológicos conforme o contexto da coleta, possibilitando análises comparativas entre os períodos operacionais.

## 8. Classificação visual das não conformidades

A representação espacial dos pontos utiliza critérios de formatação condicional baseados na quantidade acumulada de não conformidades durante o ano.

| Quantidade anual de NC | Classificação visual |
|---|---|
| 0 | 🟢 Verde |
| 1 a 2 | 🟡 Amarelo |
| 3 a 5 | 🟠 Laranja |
| 6 a 8 | 🔴 Vermelho |
| 9 ou mais | 🟣 Roxo |

Essa classificação permite identificar pontos com maior quantidade de ocorrências microbiológicas ao longo do período.

A classificação visual do histórico de não conformidades é independente do status da última análise realizada.

## 9. Monitoramento da condição mais recente

O dashboard contempla indicadores destinados à identificação:

- Da última coleta realizada.
- Da última análise microbiológica.
- Do último status de conformidade.
- Da quantidade acumulada de não conformidades.

A utilização conjunta dessas informações permite acompanhar tanto a condição microbiológica mais recente quanto o histórico de ocorrências do ponto.

## 10. Validações de higienização

As análises podem contemplar diferentes momentos do processo de higienização.

Entretanto, determinadas validações possuem dashboards específicos, como as validações de CIP (Cleaning in Place), que contemplam avaliações realizadas antes e depois da higienização.

Essa separação permite preservar as particularidades analíticas e operacionais de cada modalidade de monitoramento.

## 11. Abrangência temporal

O dashboard está direcionado ao acompanhamento dos resultados do ano de monitoramento.

A consulta comparativa entre diferentes anos não está contemplada na versão atual do projeto.

## 12. Possíveis melhorias futuras

- Implementação de indicadores de cumprimento da frequência de coleta.
- Identificação automatizada de pontos com coletas em atraso.
- Monitoramento do intervalo entre não conformidades e reverificações.
- Indicadores de reincidência microbiológica.
- Comparação histórica entre diferentes anos.
- Validação automatizada da integridade dos registros.
- Desenvolvimento de alertas para desvios de monitoramento.

## 13. Confidencialidade

A documentação apresenta as regras conceituais de funcionamento do dashboard, sem divulgar resultados laboratoriais, limites microbiológicos específicos, frequências operacionais individuais ou informações confidenciais da unidade industrial.
