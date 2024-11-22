Uma API (Interface de Programação de Aplicações, ou Application Programming Interface em inglês) é um conjunto de definições e protocolos que permite que diferentes sistemas ou programas de software se comuniquem entre si. Em termos simples, é uma maneira de um software "falar" com outro software.
-Facilita comunicação de partes diferentes do software
-Agiliza o desenvolvimento
-Tornar o código de mais qualidade
-Usando um código já testado, assegura a segurança.
Ela define as formas de interação que um desenvolvedor pode ter com um sistema, serviço ou biblioteca.

O que é uma requisição?
Para buscar ou modificar dados no servidor,  precisamos fazer requisições para as APIs.

URL/Método(HTTP:GET;POST;PUT;DELETE)/Header(cabeçalho, permite ao cliente inf. da requisição/Body (opcional da mensagem com dados)

HTTP protocolo com conj de regras para se comunicar
Método ou verbos :
GET : obter inf de um recurso pelo seu identificados ou uma lista de inf.
POST: Criar algo no recuso no servidor, mandar dados para o servidor
PUT Atualizar alguma inf no servidor
DELETE remover alguma in no servidor

POSTMAN
Ferramenta para fazer as requisições
Realizar requisições para APIs
Fazer testes automatizados

1. GET Request: Buscar todos os usuários
NEW > HTTP (não precisa de body)
Método: GET
URL: https://jsonplaceholder.typicode.com/users
Este é um exemplo de uma requisição que simplesmente retorna todos os usuários de um serviço fictício.

3. POST Request: Criar um novo usuário
NEW > HTTP > trocar para POST
Método: POST
URL: https://jsonplaceholder.typicode.com/users
Corpo (Body):
Selecione raw e escolha o formato JSON.
Adicione este conteúdo:
{
  "name": "Antonio Robert",
  "email": "antoniorobert@example.com",
  "username": "antbert"
}
PS: Pode add: ID, telefone, endereço, idade... depende da documentação da API)
Essa requisição envia um novo usuário para ser criado.

5. PUT Request: Atualizar um usuário existente
NEW > HTTP > trocar para PUT
Método: PUT
URL: https://jsonplaceholder.typicode.com/users/1 (coloque o ID do usuário)
Corpo (Body):
Selecione raw e escolha o formato JSON.
Adicione este conteúdo:
json
{
  "name": "Antonio Robert",
  "email": "antoniorobert23@example.com",
  "username": "antbert"
}
Essa requisição altera os dados de um usuário já existente.

6. DELETE Request: Excluir um usuário
NEW > HTTP > trocar para DELETE
Método: DELETE
Não precisa de BODY
URL: https://jsonplaceholder.typicode.com/users/1 (coloque o ID do usuário)
Essa requisição apaga o usuário com ID 1.

7. Testando tudo
Escolha o coleção
Clique nas "..."
Selecione "Run collection"
Clique em Run{coleção}
Irá mostrar cada API e se passou o teste ou qual "error" deu

