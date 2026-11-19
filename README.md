# Screenmatch

Aplicação de linha de comando em **Java com Spring Boot** que consome a API **OMDb** para buscar séries e analisar seus episódios. Desenvolvida durante o curso de Java da **Alura**, com foco em **Streams** e **expressões lambda**.

## Funcionalidades

- Busca de uma série pelo nome e exibição dos dados gerais
- Listagem de todas as temporadas e episódios
- Top 5 episódios mais bem avaliados
- Busca de episódio por trecho do título
- Filtro de episódios lançados a partir de um ano
- Média de avaliação por temporada e estatísticas gerais (média, melhor e pior episódio)

## Conceitos praticados

- Consumo de API REST com `HttpClient`
- Conversão de JSON para objetos Java (records) com Jackson
- Streams: `filter`, `map`, `flatMap`, `sorted`, `limit`, `peek`, `collect`
- `Collectors.groupingBy`, `averagingDouble` e `DoubleSummaryStatistics`
- `Optional` e tratamento de datas com `LocalDate`

## Tecnologias

- Java 24
- Spring Boot 3.5
- Jackson
- Maven

## Como executar

1. Gere uma chave gratuita em [omdbapi.com](https://www.omdbapi.com/apikey.aspx).
2. Defina a variável de ambiente com a sua chave:

```bash
export OMDB_API_KEY=sua-chave
```

3. Rode a aplicação:

```bash
git clone https://github.com/RicardoLMessias/screenmatch.git
cd screenmatch
./mvnw spring-boot:run
```

Depois é só digitar o nome de uma série no terminal (ex.: `gilmore girls`).

## Autor

Ricardo Lima Messias — [GitHub](https://github.com/RicardoLMessias) · [LinkedIn](https://www.linkedin.com/in/ricardolimamessias-java)
