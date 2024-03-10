# Projeto API Local de Tweets

Este projeto é uma simples API local destinada a manipular "tweets". A API permite criar novos tweets, buscar por todos os tweets existentes, deletar um tweet específico por ID e deletar todos os tweets. O projeto utiliza o framework [Gin](https://github.com/gin-gonic/gin) para roteamento e manipulação de requisições HTTP.

## Iniciando

Para começar a usar esta API, clone o repositório para sua máquina local e instale as dependências necessárias.

### Pré-requisitos

- Go (versão mais recente recomendada)
- Gin

### Instalação

Clone o repositório:

```git clone https://seu-repositorio-aqui.com```


Instale as dependências necessárias:

```go get -u github.com/gin-gonic/gin```


### Executando a API

Para iniciar a API, navegue até a pasta do projeto e execute:

go run main.go

## Uso

A API está configurada para escutar rotas sob o prefixo `/v1`. As seguintes operações estão disponíveis:

### Criar um novo tweet

- **URL**: `/v1/tweet`
- **Método**: `POST`
- **Corpo da requisição**: JSON com o formato esperado pela entidade `Tweet`. Exemplo:

```json
{
    "description": "Meu mais novo Tweet"
}
```

### Lista de Tweets

- **URL**: `/v1/tweets`
- **Método**: `GET`
- **Corpo da requisição**: Vazio. Exemplo:

```
http:.../v1/tweets
```

### Delete Tweet

- **URL**: `/v1/tweet`
- **Método**: `DELETE`
- **Corpo da requisição**: ID do tweet no Url. Exemplo:

```
http:.../v1/tweet/IDTWEET
```

### Delete todos Tweets

- **URL**: `/v1/tweet/deletAll`
- **Método**: `DELETE`
- **Corpo da requisição**: Vazio. Exemplo:

```
http:.../v1/tweet/deleteAll
```



