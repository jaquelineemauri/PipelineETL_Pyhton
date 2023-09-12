# Explorando IA Generativa em um Pipeline de ETL com Python

Neste desafio, criei um Pipeline ETL, a partir de um cenário fictício em que é necessário envolver clientes de um banco de forma personalizada, com mensagens automáticas sobre vendas de produtos financeiros utilizando uma IA Generativa (API do ChatGPT).

## Processo de Extração (Extract):
O processo inicia-se a partir da criação de um banco de dados com a API REST (_método GET_) desenvolvida na SDW 2023 **extração** dos IDs de usuários de uma planilha em formato .CSV com Pandas;


## Processo de Transformação (Transform):
Dados obtidos, foi utilizado a API do ChatGPT-4 para gerar uma mensagem de marketing personalizada para cada cliente, enfatizando a importância dos investimentos;


## Processo de Carregamento (Load):
Mensagens para cada cliente geradas, essas informações foram enviadas para a API REST utilizando a lista de "news" de cada usuário a partir do endpoint **PUT https://sdw-2023-prd.up.railway.app/users/{id}**.


### Links Úteis:
* [Documentação: API REST utilizada](https://github.com/digitalinnovationone/santander-dev-week-2023-api)
* [Documentação: API ChatGPT-4 (OpenAI)](https://platform.openai.com/docs/api-reference/introduction)
* [Link para a criação da chave](https://platform.openai.com/account/api-keys)

#

### _Mentor do projeto:_
_[@Venilton Falvo](https://github.com/falvojr) Tech Lead na [@DIO](https://github.com/digitalinnovationone)_
