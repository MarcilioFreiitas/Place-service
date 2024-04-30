


# 🌍 API de Gerenciamento de Lugares

Este é um projeto de API para gerenciar lugares (CRUD) que faz parte do desafio para desenvolvedores backend que se candidatam para a ClickBus. 🚌

## 💻 Tecnologias Utilizadas

- Spring Boot
- Spring Webflux
- Spring Data + R2DBC

## 📚 Práticas Adotadas

- SOLID
- Testes automatizados 🧪
- Consultas com filtros dinâmicos usando o Query By Example
- API reativa na web e na camada de banco
- Uso de DTOs para a API
- Injeção de Dependências
- Geração automática do Swagger com a OpenAPI 3
- Geração de slugs automática com o Slugify
- Auditoria sobre criação e atualização da entidade

## 🚀 Como Executar

### Localmente

1. Clonar repositório git 📂
2. Construir o projeto: `./mvnw clean package` 🛠️
3. Executar: `java -jar place-service/target/place-service-0.0.1-SNAPSHOT.jar` 🏃‍♂️

A API poderá ser acessada em localhost:8080. O Swagger poderá ser visualizado em localhost:8080/swagger-ui.html 🌐

### Usando Docker 🐳

1. Clonar repositório git 📂
2. Construir o projeto: `./mvnw clean package` 🛠️
3. Construir a imagem: `./mvnw spring-boot:build-image` 🖼️
4. Executar o container: `docker run --name place-service -p 8080:8080  -d place-service:0.0.1-SNAPSHOT` 🚢

A API poderá ser acessada em localhost:8080. O Swagger poderá ser visualizado em localhost:8080/swagger-ui.html 🌐

## 📡 API Endpoints

Para fazer as requisições HTTP abaixo, foi utilizada a ferramenta httpie:

- POST /places: `http POST :8080/places name="Place" state="State"` 📮
- GET /places/{id}: `http :8080/places/1` 📬
- GET /places?name=? : `http :8080/places name==PLACE` 📬
- PATCH /places/{id}: `http PATCH :8080/places/1 name='New Name' state='New State'` 📝
```
Espero que você goste! 😊
