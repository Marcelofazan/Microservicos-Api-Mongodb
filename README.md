## 🚀 Microservicos-Api-Mongodb
Exemplo de projeto API Arquitetura Distribuída em Microserviços de em C# ASP.NET 10 com banco de dados MongoDB.

#### 📋 O que você vai encontrar neste projeto

| Tecnologia | Descrição |
|-----------|-----------|
| **Arquitetura distribuída**| É um modelo executado em diferentes servidores conectados em rede, conversando entre si para parecer único sistema |
| **T Genérico**| Criar estruturas de código com diferentes tipos de dados sem precisar reescrever o código para cada um deles. |
| **Nuget**| Criação de pacote NuGet para estratégia (DRY), para evitar repetição de código no compartilhamento entre microserviços.|

#### 💬 Requisitos do Projeto
- Necessário acomplamento de serviços, o Inventário depende da execução de Catalogo.

#### 🔄 Executar a aplicação
VSCode Terminal [1]
- Executar API Catalogo para cadastro de produtos: 

| HOST | URL |
|-----------|-----------|
| **API**  |(https://localhost:7026/api/items/) |
| **Swagger** |(https://localhost:7026/swagger/index.html) |

VSCode Terminal [2]
- Executar API Inventário, ela depende de API de Catalogo.  

| HOST | URL |
|-----------|-----------|
| **API**  |(https://localhost:7012/api/Items) |
| **Swagger** |(https://localhost:7012/swagger/index.html |

#### 🧪 Executar Endpoints
- Enviar POST / Catalogo para criação do banco Entity: **https://localhost:7026/api/items/**, selecionar Guia Body e enviar RAW e enviar o seguinte Content-Type: application/json

```json
{
	"Name" : "Abacaxi",
	"Description" : "Abacaxi",
	"Price" : 6.00
}
```

- Enviar POST / Inventário para criação do banco Entity: **https://localhost:7012/api/Items**, selecionar Guia Body e enviar RAW e enviar o seguinte Content-Type: application/json
```json
{
    "UserId" : "a4ce3b13-acef-2cd2-8855-89cfaaac5224",
    "CatalogItemId" : "fe373bcd-5b51-427d-adf1-6a0771f06c16",
    "Quantity" : 80
}
```

#### ⚙️ Configuração Pacote Nuget

 O Projeto **Pacote** foi compilado e hospedado em **(nuget.org)** para ser usado no projeto com **(using Pacote)**.
 
 [Criar e publicar um pacote NuGet usando o Visual Studio](https://learn.microsoft.com/pt-br/nuget/quickstart/create-and-publish-a-package-using-visual-studio?tabs=netcore-cli)
  
