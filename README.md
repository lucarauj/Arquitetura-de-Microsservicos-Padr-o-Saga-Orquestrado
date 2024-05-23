# Curso Arquitetura de Microsserviços: Padrão Saga Orquestrado

<br>

## Microsserviços

- pequenos serviços independentes que se comunicam usando APIs

<br>

## Transações distribuídas

- iniciam em um microsserviço, mas ela só é finalizada em outro

<br>

## Two-Phase Commit Protocol (2PC)

- protocolo atômico que elabora uma estratégia para realizar um commit em duas etapas em uma transação distribuída

<br>

## Padrão Saga

- garante a execução de sucesso de um fluxo de transações
- em caso de falha, todas as alterações são desfeitas na sequência que foram realizadas

<br>

## Saga Orquestrado

- um agente externo aos microsserviços envolvidos determina qual será a ordem de envio dos eventos baseados em casos de sucesso e falha

<br>

## Saga Coreografado

- o próprio serviço possui a lógica para saber qual será o próximo passo a ser decidido no fluxo com base no resultado da iteração

<br>

## Saga Execution Controller

- objeto ou entidade controladora de execução do saga

<br>

## Padrão Outbox

- sempre que houver a necessidade de enviar um evento a um Message Broker, ao invés de realizar o envio direto no fluxo de processamento, salva o conteúdo do evento em uma tabela que represente o Outbox

<br>

