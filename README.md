🟢 **Storeflow - Microserviço de um PetShop** 🐾

🟢 **Descrição do Projeto**

**O Starflow é um sistema de microserviço voltado para gerenciamento de pedidos e serviços de um PetShop.
O projeto foi desenvolvido para demonstrar a construção de microserviços robustos, escaláveis e bem testados, usando Spring Boot 3.5.8, Java JDK 17, Maven e conteinerização via Rancher Desktop.**

**O microserviço gerencia funcionalidades como:**

Cadastro e gerenciamento de clientes e pets.

Registro e controle de pedidos de serviços do PetShop.

Comunicação entre microserviços, garantindo integração com outros sistemas.

🟢 **Tecnologias Utilizadas**

Java JDK 17

Maven como gerenciador de dependências

Spring Boot 3.5.8 (Spring Web, Spring Data JPA, Spring Test)

Banco de dados H2 (para desenvolvimento e testes)

Rancher Desktop para containerização e execução de microserviços

JUnit 5 para testes unitários

Mockito para testes de integração simulando dependências

QA e testes automatizados garantindo a qualidade do código

Estrutura de Microserviços

PetShop Microservice: Gerencia cadastro de pets, clientes e serviços do PetShop.

Starflow Microservice: Gerencia pedidos e integra com o PetShop Microservice, simulando um fluxo completo de pedidos.

Cada microserviço roda isoladamente em seu container, permitindo testes independentes e escalabilidade.

🟢 **Como Rodar o Projeto**
Pré-requisitos:

Rancher Desktop instalado

Docker funcionando dentro do Rancher Desktop

JDK 17

Maven

Comandos

🟢 **Subir todos os microserviços:**

./mvnw spring-boot:run

ou, se usar containers via Rancher:

docker-compose up -d

🟢 **Pausar o projeto:**

docker-compose pause

Retomar o projeto:

docker-compose unpause

🟢 **Interromper/Parar o projeto:**

docker-compose down

🟢 **Testes Automatizados**

**O projeto possui testes para garantir estabilidade e confiabilidade:**

**Testes Unitários: usando JUnit 5, verificando funcionalidades isoladas.**

**Testes de Integração: usando Mockito, garantindo que os microserviços se comuniquem corretamente.** 🚀
