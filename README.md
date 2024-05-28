# Aplicação CRUD Fullstack
Esta é uma aplicação CRUD (Create, Read, Update, Delete) fullstack construída com React, Axios, Toastify, Express e MySQL. A aplicação permite cadastrar, deletar, atualizar e exibir informações de usuários, incluindo nome, email, telefone e data de nascimento.

## Índice

- [Recursos](#recursos)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Instalação](#instalação)
- [Uso](#uso)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Contribuindo](#contribuindo)
- [Licença](#licença)

## Recursos

- **Create**: Cadastrar novos usuários com nome, email, telefone e data de nascimento.
- **Read**: Exibir uma lista de usuários cadastrados.
- **Update**: Editar informações de usuários.
- **Delete**: Remover usuários do banco de dados.
- **Notificações**: Exibir mensagens de sucesso e erro usando Toastify.

## Tecnologias Utilizadas

- **Frontend**:
  - React
  - Axios
  - Toastify
  - Styled Components

- **Backend**:
  - Express
  - MySQL
  - Nodemon (para desenvolvimento)

## Instalação

### Pré-requisitos

- Node.js (v14 ou posterior)
- Servidor MySQL

### Configuração do Backend

1. Clone o repositório:

   ```bash
   git clone [https://github.com/seu-usuario/seu-repo.git](https://github.com/rodericussilva/fullstack-crud-react.git)
   cd crud
    ```
2. Navegue até o diretório backend:
   ```bash
   cd api
   ```
3. Instale as dependências do backend:
   ```bash
   yarn stall
   ```
4. Configure seu banco de dados MySQL:
- Crie um novo banco de dados MySQL.

- Execute o seguinte script SQL para criar a tabela usuarios:
  ```sql
  CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(255) NOT NULL,
  email VARCHAR(255) NOT NULL,
  phone VARCHAR(20),
  date_born DATE
); ```

5. Inicie o servidor backend:
   ```bash
   yarn start
   ```

### Configuração do Frontend

1. Navegue até o diretório `frontend`:
   ```bash
   cd frontend
   ```

2. Instale as dependências do frontend:
   ```bash
   yarn install
   ```
3. Incie o servidor frontend:
    ```bash
    yarn start
    ```
A aplicação deve estar rodando em `http://localhost:3000` para o frontend e `http://localhost:8800` para o backend.

## Uso
- Abra seu navegador e navegue até http://localhost:3000.
- Use o formulário para cadastrar novos usuários.
- Veja a lista de usuários cadastrados.
- Use o botão de editar para atualizar as informações dos usuários.
- Use o botão de deletar para remover usuários da lista.

## Estrutura do Projeto
```plaintext
crud/
├── api/
│   ├── controllers/
│   │   └── user.js
│   ├── routes/
│   │   └── users.js
│   ├── db.js
│   └── index.js
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Form.js
│   │   │   ├── Grid.js
│   │   ├── styles/
│   │   │   └── global.js
│   │   ├── App.js
│   │   ├── index.js
|   |   ├── reporWebVitals.js
|   |   └── setupTests.js
│   └── public/
│       └── index.html
└── README.md
```

## Contribuindo

Contribuições são bem-vindas! Por favor, abra uma issue ou envie um pull request para quaisquer mudanças.

## Licença
Este projeto está licenciado sob a Licença MIT. Veja o arquivo [LICENSE](./LICENSE) para mais detalhes.

## Autor

### Rodrigo Silva

Se você tiver alguma dúvida ou sugestão, sinta-se à vontade para entrar em contato comigo em rodericus@alu.ufc.br
