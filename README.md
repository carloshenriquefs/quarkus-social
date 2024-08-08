# 🚧 - API's Quarkus Social

- Uma rede social simples, onde os usuários podem enviar textos pequenos e podem seguir uns aos outros;

##

## 📌 - Objetivos:

### 🧑‍💻 - USERS:

- Deseja-se fazer o cadastro dos usuários da redes social, o usuário envia algumas informações básicas para fazer seu cadastro.
Haverá um endpoint para listagem de usuários.

### 📲- POSTS:

- Representam as postagens dos usuários, que serão em formato de um texto curto e a data-hora. Só poderá visualizar as postagens
os seguidores do usuário.

### 📱- FOLLOWERS: 

- Os usuários poderão ter seguidores e também seguir outros usuários para que possa visualizar suas postagens. Haverá opção de deixar
de seguir o usuário.

##

## 📂 - Estrutura de Pastas:
```
├── quarkussocial
│   ├── domain
│   |  ├── model
│   |  ├── repository
│   ├── rest
│   |  ├── rest
│   |  |   ├── dto
│   |  |   ├── resource
├── tests
```

## 

## ⚙️ - Tecnologias: 

<div align="left">
  <img src="https://skillicons.dev/icons?i=java" height="40" alt="java logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=docker" height="40" alt="docker logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" height="40" alt="postgresql logo"  />
</div>

##

## 🖌️ - Funcionalidades:
- **Cadastrar Usuarios**:
- **Listar Usuário**:
- **Atualizar Usuário**:
- **Deletar Usuário**:
- **Realizar Postagens dos Usuários**:
- **Seguir Usuários**:
- **Para de Seguir Usuários**:

##

## 📜 - Documentação:

[URL Swagger](https://localhost:8080/q/swagger-ui)

##

## 🏃 - Subir a aplicação:

```shell script
./mvnw compile quarkus:dev
```

## 📦 - Empacotando aplicação:

```shell script
java -jar ./target/quarkus-app/quarkus-run.jar
```

```shell script
mvn clean package -DskipTests
```

## 🏃- Subindo a aplicação com Docker:

```shell script
docker build -f src/main/docker/Dockerfile.jvm -t quarkus-social:1.1 .
```

```shell script
docker run -i --rm -p 8080:8080 --name quarkus-social-h2 quarkus-social:1.1
```
