# Projeto tutorial blazor
projeto de tutorial da microsoft sobre o blazor

## Ambiente
- ter o .NET core 5.0
  - windows: já possui de forma nativa
  - linux: é necessário baixar
  - mac: necessário baixar
- utilizar o Visual Studio ou _Visual Studio Code_
  - _Visual Studio Code_, só vai ser necessário adicionar algumas extensões se for desenvolver, utilizei as seguintes:
    - [C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp): para debug e etc.
    - [Auto-Using for C#](https://marketplace.visualstudio.com/items?itemName=Fudge.auto-using): intelisense para C#
    - [C# Extensions](https://marketplace.visualstudio.com/items?itemName=jchannon.csharpextensions): C# IDE Extensions

## Iniciando aplicação
- iniciar aplicação
  ```
  dotnet watch
  ```

## Estrutura
- [`Program.cs`](./Program.cs) -> é o ponto de entrada da aplicação que inicia o servidor, configurações de services e middlewares.
- [`App.razor`](./App.razor) -> é o componente root do app.
- diretório [`Pages`](./Pages) -> possui as paginas web da aplicação
- [`BlazorApp.csproj`](./BlazorApp.csproj) -> define o BlazorApp e as dependencias que terá nele.
- [`launchSettings.json`](./Properties/launchSettings.json) -> responsável pela config de variáveis de ambiente.

## Anotações
- CSS
  - para criar classes CSS unicamente para o componente é necessário criar um arquivo no seguinte formato `NomeComponente.razor.css`. Ex: [Index.razor.css](Pages/Index.razor.css)
  

### Referências
- [tutorial projeto](https://dotnet.microsoft.com/en-us/learn/aspnet/blazor-tutorial/create)
- [instalação .NET linux](https://docs.microsoft.com/pt-br/dotnet/core/install/linux?WT.mc_id=dotnet-35129-website)