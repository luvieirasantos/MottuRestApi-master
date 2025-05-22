
# 🚀 API Mottu - ASP.NET Core + Oracle

![.NET](https://img.shields.io/badge/.NET-8.0-blueviolet)
![EF Core](https://img.shields.io/badge/Entity--Framework-Core-blue)
![Oracle](https://img.shields.io/badge/Database-Oracle-orange)
![Status](https://img.shields.io/badge/Status-100%25%20Funcional-success)

---

## 📋 Descrição

API RESTful desenvolvida em **ASP.NET Core 8.0** com **Entity Framework Core** e banco de dados **Oracle**, para o cadastro e gerenciamento de motos.  
A aplicação oferece endpoints completos com suporte a operações `GET`, `POST`, `PUT` e `DELETE`, além de documentação automática gerada com Swagger.

---

## 🔁 Endpoints da API

| Método | Rota                         | Descrição                        |
|--------|------------------------------|----------------------------------|
| GET    | `/api/motos`                | Lista todas as motos             |
| GET    | `/api/motos/{id}`           | Retorna uma moto pelo ID         |
| GET    | `/api/motos/busca?marca=x`  | Busca motos por marca            |
| POST   | `/api/motos`                | Cadastra uma nova moto           |
| PUT    | `/api/motos/{id}`           | Atualiza os dados de uma moto    |
| DELETE | `/api/motos/{id}`           | Remove uma moto do sistema       |

> A documentação completa está disponível via Swagger após iniciar o projeto.

---

## 🛠️ Como executar o projeto localmente

### 🔧 Pré-requisitos

- [.NET SDK 8.0](https://dotnet.microsoft.com/download/dotnet/8.0)
- Banco de dados Oracle (local ou remoto)
- Visual Studio ou Visual Studio Code

### 🚀 Passo a passo

1. **Clone este repositório:**

   ```bash
   git clone https://github.com/seu-usuario/MottuRestApi.git
   ```

2. **Configure a string de conexão no `appsettings.json`:**

   ```json
   "ConnectionStrings": {
     "OracleDb": "User Id=usuario;Password=senha;Data Source=localhost:1521/XEPDB1"
   }
   ```

3. **Aplique as migrations:**

   ```bash
   dotnet ef database update
   ```

4. **Rode a aplicação:**

   ```bash
   dotnet run
   ```

5. **Acesse o Swagger no navegador:**

   ```
   http://localhost:5000/swagger
   ```

---

## 🧰 Tecnologias Utilizadas

- ✅ ASP.NET Core 8.0
- ✅ Entity Framework Core
- ✅ Oracle Database
- ✅ Swagger / Swashbuckle.AspNetCore
- ✅ C#

---

## ✅ Funcionalidades Implementadas

- [x] API REST com padrão CRUD
- [x] Integração com Oracle via EF Core
- [x] Migrations com criação de tabelas
- [x] Documentação automática com Swagger
- [x] Filtro de busca por marca
- [x] Validação e tratamento de erros
- [x] Ambiente configurável via `appsettings.json`

---

## 📷 Captura de Tela (Swagger)

> A interface Swagger mostra todos os endpoints disponíveis e permite testá-los diretamente no navegador.

![Swagger UI](./docs/swagger-ui.png)

---

## 👤 Autores

Melissa Pereira
Lu Vieira
Diego Furigo

---

