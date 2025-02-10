# Gerenciador de Podcasts
Este é um projeto que implementa um API RESTful para gerenciar podcasts e episódios. A aplicação permite listar todos os episódios de podcasts 
disponíveis e filtrar episódios por nome de podcast.

## Funcionalidades
Listar episódios: Recupera todos os episódios de podcasts disponíveis.
Filtrar episódios: Permite a busca por episódios de um podcast específico utilizando parâmetros de consulta (query string).

## Arquitetura
O sistema é composto por várias camadas:

* Controladores: Responsáveis por processar as requisições HTTP e interagir com os serviços de negócios.
* Serviços: Contêm a lógica de negócios, como a filtragem de podcasts e a listagem dos episódios.
* Repositórios: Interagem com os arquivos, recuperando as informações necessárias sobre os podcasts.
* Modelos: Definem as estruturas de dados, como os objetos que representam os podcasts e episódios.

## Tecnologias
* TypeScript: Linguagem de programação utilizada para o desenvolvimento do projeto.
* Tsup: Ferramenta de construção e empacotamento para projetos TypeScript.
* Tsx: Compilador TypeScript que suporta a construção de projetos.
* Node.js: Ambiente de execução JavaScript que permite executar código JavaScript do lado do servidor.
* @types/node: Pacote de definições de tipos para Node.js para auxiliar no desenvolvimento com TypeScript.

## Endpoints
1. GET /api/list
Retorna uma lista de todos os episódios de podcasts.

2. GET /api/podcasts
Filtra os episódios pelo nome do podcast.

Exemplo de resposta:
````[
  {
    "podcastName": "flow",
    "episode": "CBUM - Flow #319",
    "videoId": "pQSuQmUfS30",
    "cover": "https://i.ytimg.com/vi/pQSuQmUfS30/maxresdefault.jpg",
    "link": "https://www.youtube.com/watch?v=pQSuQmUfS30",
    "categories": ["saúde", "esporte", "bodybuilder"]
  }
 ]
````
## Como Utilizar
1. Clone este repositório.
2. Instale as dependências usando npm install.
3. Inicie o servidor executando start:dev.
4. Acesse os endpoints fornecidos para listar os episódios de podcasts ou filtrá-los por nome de podcast.
