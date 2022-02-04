## ⚒ Automação API Cypress
- Projeto de automação de Api utilizando Cypress.

## 📋 Descrição 
- Utilizando a [API](https://fakerestapi.azurewebsites.net/index.html), foi realizado a automação das requisições de
Livros.

- Para automação dos testes foi utilizado o Framework [Cypress](https://www.cypress.io/).

- Utilizado o [Allure Reports](hhttps://docs.qameta.io/allure/#_installing_a_commandline), como gerenciador de relatórios.

## 🚀Instalação
### Pré-requisitos
- Fazer a instalação do [Node.Js](https://nodejs.org/en/) (recomendado seguir o guia no site oficial)
- Para a instalação do [Cypress](https://www.cypress.io/):
```
 npm install --save-dev cypress 
```

### Instalando Depedências
- Com o Node.Js e o Cypress devidamente instalados em sua máquina, acesse o diretório do projeto pelo **cmd** ou **powershell** e digite os comandos abaixo:

### Configurando [Allure Reports](https://docs.qameta.io/allure/)
- Utilizando o [Scoop](https://scoop.sh/) rode:
```
 scoop install allure
```
- Na raiz do projeto:
```
 npm i -D @shelex/cypress-allure-plugin
```
- Inserir no arquivo /plugins/index.js:
```
const allureWriter = require('@shelex/cypress-allure-plugin/writer');

module.exports = (on, config) => {
    allureWriter(on, config);
    return config;
};
```
- Inserir no arquivo /support/index.js :
```
import '@shelex/cypress-allure-plugin';
require('@shelex/cypress-allure-plugin');
```

- Após esses comandos serem digitados será instalado todas as dependências necessárias para a execução do projeto.

### Executando os testes
- Para a execução do teste utilize o comando abaixo:
```
npm run test
```
- Para exibir o relatório com Allure report:
```
npm run allure:open
```
## 📌 Autor/Contato

| [<img src="https://avatars1.githubusercontent.com/u/62215470?s=460&u=c6dc439e77463ced6dd781733712708b5fbdde65&v=4" width=115><br><sub>@Guilhermelima3</sub>](https://github.com/Guilhermelima3) |
| :---: |


- Linkedin  [Guilherme Lima](https://www.linkedin.com/in/guilherme-lima-marinho/)
- [E-mail](guilhermel_ima@hotmail.com)
---
