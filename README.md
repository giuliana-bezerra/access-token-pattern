<h1 align="center">
  Access Token Pattern
</h1>

<p align="center">
 <img src="https://img.shields.io/static/v1?label=Youtube&message=@giulianabezerra&color=8257E5&labelColor=000000" alt="@giulianabezerra" />
 <img src="https://img.shields.io/static/v1?label=Tipo&message=Tutorial&color=8257E5&labelColor=000000" alt="Tutorial" />
</p>

Projeto apresentado [nesse vídeo](https://youtu.be/lWLffhSjxZc) que demonstra o uso do access token pattern com Spring Boot e Spring Cloud Gateway.

## Configuração do Keycloak

1 - Executar Keycloak
```
docker run -p 8080:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:22.0.5 start-dev
```

2 - Criar um realm

3 - Criar usuário e client oauth no Keycloak

4 - Ajustar as propriedes do gateway para apontar pro realm e client cadastrados

5 - Executar projetos gateway e resource-server

## Testando a Aplicação

Será possível acessar uma rota protegida através do gateway em [http://localhost:9000/api/hello](http://localhost:9000/api/hello):

- GET /hello: Rota que pede autenticação