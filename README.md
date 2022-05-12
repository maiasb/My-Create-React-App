# `INICIANDO UM PROJETO REACT`

## Iniciar o package.json do react:
- $ `yarn init -y`

## Iniciar o react:
- $ `yarn add react`
- $ `yarn add react-dom`

## Criar estrutura de pastas:
- public/
    - index.html
- src/
    - index.jsx

## Instalar o babel como dependência de desenvolvimento:
- $ `yarn add @babel/core @babel/cli @babel/preset-env @babel/preset-react -D`
- $ `yarn add babel-loader -D`

- Note: preset-env permite compilar com compatibilidade em todos os ambientes especificados.
- Note: preset-react permite que o babel interprete o html no arquivo jsx.
- Note: babel-loader integra o babel ao webpack.

## Criar o arquivo 'babel.config.js e exportar módulo de configuração do babel'

## Dist com o babel:
- & `yarn babel src/index.jsx -o dist/bundle.js`

## Instalar webpack e webpack-cli como dependência de desenvolvimento:
- $ `yarn add webpack webpack-cli -D`

## Para remover a div script do html:
- $ `yarn add html-webpack-plugin -D`
- Depois, adicionar a configuração no webpack.config.js

## `REASSISTIR ESTA AULA`
### Criar o arquivo 'webpack.config.js' e exportar os módulos de configuração

### Estrutura do projeto para renderização:
- public/index.html: Onde será importado o script gerado pelo webpack 'bundle.js' e a div 'root'
- src/App.jsx: receberá as páginas da aplicação, assim como suas rotas.
- src/index.jsx será utilizada para integrar o 'App' ao 'html', na div 'root'.

### Automatizar atualização do código:
- $ `yarn add webpack-dev-server -D`
- Feito isso, para executar a aplicação: $ `yarn webpack serve`

- Obs: devServer precisa estar como static.