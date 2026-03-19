# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 19/03/2026
Empresa: Abstergo Industries
Responsável: Pedro Brandão Leal dos Santos

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado pelo Analista de Engenharia de Dados. O objetivo do projeto foi elencar 3 serviços AWS com a finalidade de realizar diminuição de custos imediatos, eliminando a dependência de infraestrutura on-premise e otimizando os gastos operacionais com tecnologia.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:



### Etapa 1:
- **Nome da ferramenta:** Amazon EC2 com Auto Scaling
- **Foco da ferramenta:** Redução de custos com infraestrutura de servidores
- **Descrição de caso de uso:** Anteriormente, a Abstergo Industries mantinha servidores físicos on-premise com capacidade máxima alocada 24/7, gerando custos fixos elevados mesmo em períodos de baixa demanda. Com a migração para o Amazon EC2 combinado com Auto Scaling, a empresa passou a provisionar instâncias apenas conforme a demanda real, escalando horizontalmente nos picos de uso e reduzindo automaticamente nos períodos ociosos. O modelo de pagamento **pay-as-you-go** eliminou os gastos com hardware ocioso, resultando em redução estimada de 40% nos custos de infraestrutura.



### Etapa 2:
- **Nome da ferramenta:** Amazon S3 + S3 Intelligent-Tiering
- **Foco da ferramenta:** Otimização de custos de armazenamento de dados
- **Descrição de caso de uso:** A empresa armazenava grandes volumes de dados históricos em servidores locais com alto custo de manutenção e risco de perda. Com a migração para o Amazon S3 e a ativação do **S3 Intelligent-Tiering**, os dados passaram a ser movidos automaticamente entre camadas de armazenamento (frequente, infrequente e arquivo) com base no padrão de acesso. Dados raramente acessados são armazenados em camadas mais baratas como o **S3 Glacier**, reduzindo o custo de armazenamento em até 70% em comparação ao modelo on-premise, sem qualquer perda de disponibilidade ou durabilidade.



### Etapa 3:
- **Nome da ferramenta:** AWS Lambda
- **Foco da ferramenta:** Eliminação de custos com servidores dedicados para processamento de tarefas
- **Descrição de caso de uso:** Diversos processos internos da Abstergo Industries (geração de relatórios, processamento de notificações, integração entre sistemas) eram executados em servidores dedicados que ficavam ociosos a maior parte do tempo, gerando custos desnecessários. Com a adoção do **AWS Lambda**, esses processos foram convertidos em funções serverless executadas sob demanda. A empresa passou a pagar apenas pelo tempo de execução real de cada função (em milissegundos), eliminando completamente o custo de servidores ociosos. A estimativa de economia é de 60% em relação ao modelo anterior para esse tipo de carga de trabalho.



## Conclusão
A implementação de ferramentas na empresa **Abstergo Industries** tem como esperado a **redução significativa de custos operacionais de TI**, eliminação de desperdícios com infraestrutura ociosa e maior flexibilidade para escalar conforme a demanda do negócio. A combinação de **EC2 com Auto Scaling**, **Amazon S3 com Intelligent-Tiering** e **AWS Lambda** representa uma arquitetura moderna, resiliente e econômica, alinhada às melhores práticas de Cloud Computing. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias — como Amazon RDS, CloudFront e AWS Cost Explorer — que possam melhorar ainda mais os processos e a visibilidade de custos da empresa.



## Anexos

- Manual de configuração do Amazon EC2 Auto Scaling
- Política de ciclo de vida do Amazon S3 Intelligent-Tiering
- Documentação das funções AWS Lambda implementadas
- Relatório comparativo de custos: on-premise vs AWS (antes e depois)
- Diagrama de arquitetura da solução implementada



Assinatura do Responsável pelo Projeto:

**Analista de Engenharia de Dados**
Pedro Brandão Leal dos Santos
