# Gabriel Henrique Costa

### Desenvolvedor Backend | Java & Spring Boot

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gabrielhpcosta)
[![Gmail](https://img.shields.io/badge/gabehpc@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:gabehpc@gmail.com)

Oi! Sou estagiário de desenvolvimento backend com Java e curso Ciência da Computação. Moro em Campinas, SP.

No estágio trabalho com integrações entre sistemas, e nos projetos pessoais uso Spring Boot para colocar em prática o que vou aprendendo. Gosto de entender as regras do negócio antes de escrever código e de deixar a API pronta para os casos que dão errado, não só para o caminho feliz.

## Com o que trabalho

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![Mockito](https://img.shields.io/badge/Mockito-78A641?style=for-the-badge)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

## Projetos

### [RestauranteAPI](https://github.com/gabrielhpcosta/RestauranteAPI)

É o projeto em que mais investi até agora. Uma API para o dia a dia de um restaurante: o garçom abre a comanda na mesa, lança os pedidos, a cozinha vai mudando o status de cada item e, no fim, a conta é paga e a comanda fechada.

Algumas coisas que precisei resolver no caminho:

- Se a internet cai e o garçom manda o pagamento de novo, a conta não pode ser cobrada duas vezes. Cada pagamento tem uma chave de idempotência, e a mesma chave sempre devolve o pagamento que já existe.
- Dois pagamentos chegando ao mesmo tempo podiam deixar a conta paga a mais. Resolvi travando a comanda no banco durante o pagamento.
- O estoque baixa sozinho pela receita de cada produto quando o pedido entra, e volta quando um item é cancelado.
- Um funcionário desligado perde o acesso na hora, mesmo que ainda tenha um token válido.

Tem 23 testes automatizados com JUnit e Mockito e a documentação fica no Swagger.

Java 17, Spring Boot 4, Spring Security com JWT, PostgreSQL e Docker.

### [ClinicaAPI](https://github.com/gabrielhpcosta/ClinicaAPI)

API para gestão de clínicas: pacientes, médicos, especialidades e consultas. Antes de marcar uma consulta, ela confere se o médico tem horário livre naquela data. O acesso é separado entre administrador e recepcionista, o login bloqueia depois de várias tentativas erradas e o endereço do paciente é preenchido pelo CEP usando o ViaCEP.

Java 17, Spring Boot, Spring Security com JWT, PostgreSQL e Swagger.

### [APIAgendamento](https://github.com/gabrielhpcosta/APIAgendamento)

Uma API de agendamentos mais simples, que fiz para praticar a estrutura básica de uma API REST com Spring Data JPA.

## O que estou estudando agora

Quero colocar CI com GitHub Actions nos meus projetos, aprender mensageria com RabbitMQ ou Kafka para integrar sistemas de forma assíncrona e começar a escrever testes de integração com Testcontainers.
