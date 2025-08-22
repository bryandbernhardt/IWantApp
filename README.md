# IWantAPI
![dotnet](https://github.com/BryanDietrichBernhardt/IWantApp/blob/master/Assets/dot-net-banner.png)


![GitHub repo size](https://img.shields.io/github/repo-size/BryanDietrichBernhardt/IWantApp?style=for-the-badge)
![GitHub language count](https://img.shields.io/github/languages/count/BryanDietrichBernhardt/IWantApp?style=for-the-badge)
<!---![GitHub forks](https://img.shields.io/github/forks/BryanDietrichBernhardt/IWantApp?style=for-the-badge)
![Bitbucket open issues](https://img.shields.io/bitbucket/issues/BryanDietrichBernhardt/IWantApp?style=for-the-badge)
![Bitbucket open pull requests](https://img.shields.io/bitbucket/pr-raw/BryanDietrichBernhardt/IWantApp?style=for-the-badge)--->

<!--- <img src="exemplo-image.png" alt="exemplo imagem"> --->

> API de pedidos de produtos desenvolvida em .NET 6.
### Ajustes e melhorias

O projeto ainda está em desenvolvimento e as próximas atualizações serão voltadas nas seguintes tarefas:

- [x] Estruturação inicial de endpoints
- [x] Conexão com SQL Server
- [x] Validações com Flunt
- [x] Identity
- [x] Autenticação
- [x] Logs
- [x] Gerenciamento de Produto
- [x] Vitrine de Produto
- [x] Gerenciamento de Cliente
- [x] Pedido
- [x] Configurar Docker

## 💻 Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:
<!---Estes são apenas requisitos de exemplo. Adicionar, duplicar ou remover conforme necessário--->
* Frameworks `.NET 6`
* Banco de Dados `SQL Server 2019`
* Docker `(Não obrigatório)`

## 🚀 Rodando IWantAPI

Agora a API está "Dockerizada"!<br>
Obs: Necessário configurar container para conexão com o banco de dados.<br>
Para criar e rodar a imagem no ambiente de desenvolvimento:
```
docker build .
docker images
docker run -it --rm -p 8000:80 --name IWantAPI --env ASPNETCORE_ENVIRONMENT=Development <imagem>
```
<br>
Para rodar a API em um PC local, siga estas etapas:<br>
Linux/macOS/Windows:<br>
1 - Verifique a string de conexão do banco em appsettings.Development.json (Atualize com o seu SQL Server)<br>
2 - Execute as Migrations<br>
3 - Build/Run<br>

```
dotnet ef database update
dotnet build
dotnet run
```

## ☕ Usando a API

Como padrão do .NET, pode-se testar os endpoints com o próprio Swagger ou softwares externos (Postman/Insomnia)

[⬆ Voltar ao topo](#IWantAPI)<br>
