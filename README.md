<p align="center"><img width="500px" src="https://github.com/lucarauj/Arquitetura-de-Microsservicos-Padrao-Saga-Orquestrado/blob/main/Images/Imagem Curso.png" /></p>

# Arquitetura de Microsserviços: Padrão Saga Orquestrado

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

## Event-Driven Architecture (EDA) ou Arquitetura Orientada a Eventos

- estilo de arquitetura de software em que a troca de informações e a coordenação de componentes são baseadas em eventos
- não possui uma implementação física, e sim é um desenho arquitetural

<br>

## Apache Kafka 

- ecossistema de streaming de eventos de maneira distribuída

<br>

## Idempotência

- ações que podem ser repetidas várias vezes sem causar efeitos colaterais adicionais ou alterar o resultado final além da primeira execução

<br>

# Arquitetura do projeto

<p align="center"><img width="600px" src="https://github.com/lucarauj/Arquitetura-de-Microsservicos-Padrao-Saga-Orquestrado/blob/main/Images/Arquitetura Proposta.png" /></p>

<br>

## Tecnologias utilizadas no projeto

- Git/GitHub
- IntelliJ
- Java 17
- Docker
- Dbeaver
- PostgreSQL
- MongoDB
- Kafka
- Gradle
- Redpanda

<br>

## Dependências:

- spring-web
- spring-data-jpa
- kafka
- lombok
- devtools
- springdoc-openapi
- validation
- postgresql

<br>

## Criando imagens Docker

- docker-compose up --build -d

<br>

## Anotações

- @AllArgsConstructor
- @Bean
- @Builder
- @Component
- @Configuration
- @ControllerAdvice
- @Data
- @Document
- @EnableKafka
- @ExceptionHandler
- @Getter
- @Id
- @KafkaListener
- @NoArgsConstructor
- @RequiredArgsConstructor
- @ResponseStatus
- @Service
- @Slf4j
- @Value

<br>

## Compilando o código fonte

- ./gradlew build

<br>

## Removendo containers

- docker-compose down

<br>

# 👨🏼‍🎓 Aluno

Lucas Araujo

<a href="https://www.linkedin.com/in/lucarauj"><img alt="lucarauj | LinkdeIN" width="40px" src="https://user-images.githubusercontent.com/43545812/144035037-0f415fc7-9f96-4517-a370-ccc6e78a714b.png" /></a>

