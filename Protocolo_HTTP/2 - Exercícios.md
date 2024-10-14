# Lista de Exercícios - Protocolos HTTP e HTTPS com Postman

## Objetivo
Praticar o uso dos principais métodos HTTP e explorar os conceitos de requisições web seguras (HTTPS) utilizando a ferramenta **Postman**.

---

### Guia de Instalação do Postman

1. Acesse o site oficial do Postman: [https://www.postman.com/downloads/](https://www.postman.com/downloads/).
2. Baixe a versão adequada para o seu sistema operacional (Windows, macOS ou Linux).
3. Siga as instruções de instalação fornecidas pela Postman.
4. Após instalar, crie uma conta ou use o modo offline para começar a explorar.

---

## Exercícios

### 1. **Requisições HTTP Básicas**

#### a. **GET**:
- Abra o Postman e crie uma nova requisição.
- Defina o método como `GET` e insira o seguinte URL: `https://jsonplaceholder.typicode.com/posts/1`.
- Clique em **Send** e examine a resposta.
- **Pergunta**: Quais são os principais elementos retornados na resposta (status code, corpo, cabeçalhos)?

#### b. **POST**:
- No Postman, altere o método para `POST` e use o seguinte URL: `https://jsonplaceholder.typicode.com/posts`.
- No corpo da requisição, selecione o formato **raw** e escolha **JSON**. Insira os seguintes dados:
  
  ```json
  {
    "title": "Estudando HTTP",
    "body": "Este é um exemplo de requisição POST.",
    "userId": 1
  }
  ```
- Clique em **Send**.
- **Pergunta**: Qual foi a resposta do servidor após o envio do POST?

#### c. **PUT**:
- Altere o método para `PUT` e use o URL `https://jsonplaceholder.typicode.com/posts/1`.
- Envie os seguintes dados no corpo da requisição:

  ```json
  {
    "id": 1,
    "title": "Atualização de Post",
    "body": "Atualizando um post com PUT.",
    "userId": 1
  }
  ```
- **Pergunta**: O que mudou na resposta em comparação com o POST?

#### d. **DELETE**:
- Alterar o método para `DELETE` e use o URL `https://jsonplaceholder.typicode.com/posts/1`.
- Clique em **Send**.
- **Pergunta**: O que acontece quando tentamos deletar um recurso?

---

### 2. **Explorando HTTPS**

1. Faça uma requisição `GET` para o seguinte site seguro: `https://api.github.com/`.
2. Verifique os detalhes da resposta e identifique se a comunicação foi feita via HTTPS (indicado por um cadeado no Postman).
   
   **Pergunta**: Como o uso de HTTPS garante a segurança dos dados transmitidos?

---

### Entrega

- Suba suas respostas e prints das telas no seu repositório GitHub em uma pasta chamada `exercicios-http-postman`.
- Inclua um arquivo `README.md` descrevendo cada exercício e os passos realizados no Postman.
- Lembrando que toda a atividade de portfólio é considerada parte da avaliação da disciplina.
