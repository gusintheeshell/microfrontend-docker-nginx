<h1>FazenTECH</h1>

<p align="center">
  <img src="https://img.shields.io/static/v1?label=REACT%20NATIVE&message=FRAMEWORK&color=00BEF5&style=for-the-badge&logo=REACT"/>
  <img src="https://img.shields.io/static/v1?label=REACT%20JS&message=LIBRARY&color=0597ff&style=for-the-badge&logo=REACT"/>
  <img src="https://img.shields.io/static/v1?label=NODEJS&message=Runtime%20Built&color=339933&style=for-the-badge&logo=Node.js"/>
  <img src="https://img.shields.io/static/v1?label=JAVASCRIPT&message=Language&color=F7DF1E&style=for-the-badge&logo=javascript"/>
  <img src="http://img.shields.io/static/v1?label=License&message=MIT&color=green&style=for-the-badge"/>
  <img src="http://img.shields.io/static/v1?label=TESTES&message=%3E100&color=GREEN&style=for-the-badge"/>
  <img src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=RED&style=for-the-badge"/>
</p>

> Status do Projeto: :warning: (em desenvolvimento)

### Tópicos

:small_blue_diamond: [Descrição do projeto](#descrição-do-projeto)

:small_blue_diamond: [Contextualização do PTG](#contextualização-do-ptg)

:small_blue_diamond: [Funcionalidades](#funcionalidades)

:small_blue_diamond: [Layout da Aplicação](#layout-da-aplicação-dash)

:small_blue_diamond: [Pré-requisitos](#pré-requisitos)

:small_blue_diamond: [Como rodar a aplicação](#como-rodar-a-aplicação-arrow_forward)

## Descrição do projeto

<p align="justify">
Trabalho interdisciplinar do 5º Semestre do curso de Análise e Desenvolvimento de Sistemas. A tarefa é desenvolver um aplicativo, que inicialmente funcionará apenas em dispositivos Android. Mas antes de chegar ao produto que será disponibilizado aos usuários, será preciso
desenvolver uma espécie de protótipo funcional, com uma interface próxima à final, e contendo as
principais funcionalidades e recursos, mas sem se preocupar ainda com métodos de pagamento ou
a comunicação com o servidor e banco de dados da fazenda.
</p>
<p>E como extra, fizemos o backend (api) e uma versão web.</p>

## Contextualização do PTG

Uma das principais fontes de renda da fazenda de Lúcia é a venda do que ela produz, como o leite,
legumes, verduras, entre outros produtos. Com a informatização da fazenda, tudo está ligado a um
sistema robusto, capaz de gerenciar cada atividade e produções da fazenda, como por exemplo,
controlar seus produtos e estoques.
Lúcia vende em atacado para grandes varejistas, de forma tradicional, porém ela gostaria de expandir
o negócio, e começar a oferecer seus produtos ao consumidor final! Para este fim, ela precisa de um
aplicativo mobile para que os consumidores possam visualizar todo seu catálogo de produtos, efetuar
seus pedidos, pagar e agendar a entrega.

## Funcionalidades

:heavy_check_mark: Funcionalidade 1

:heavy_check_mark: Funcionalidade 2

:heavy_check_mark: Funcionalidade 3


## Layout da Aplicação :dash:

<table align="center">
	<tr align="center"><td><img src="https://github.com/gusbdev/FazenTECH/blob/master/media-project/screenshots/app/Screenshot_20201030-221332.png" width="300" height="500" /><br /><sub>Tela inicial</sub></td><td><img src="https://github.com/gusbdev/FazenTECH/blob/master/media-project/screenshots/app/Screenshot_20201030-221346.png" width="300" height="500" /><br /><sub>Tela de login</sub></td><td><img src="https://github.com/gusbdev/FazenTECH/blob/master/media-project/screenshots/app/Screenshot_20201030-221354.png" width="300" height="500" /><br /><sub>Tela de cadastro de usuário</sub></td></tr>
	<tr align="center"><td><img src="https://github.com/gusbdev/FazenTECH/blob/master/media-project/screenshots/app/Screenshot_20201030-221629.png" width="300" height="500" /><br /><sub>Tela com os produtos listados</sub></td><td><img src="https://github.com/gusbdev/FazenTECH/blob/master/media-project/screenshots/app/Screenshot_20201030-223038.png" width="300" height="500" /><br /><sub>Tela de checkout</sub></td></tr>
</table>

<caption>(Versão Web)</caption>
<p align="center">
<img src="https://github.com/gusbdev/FazenTECH/blob/master/media-project/web-login-register.gif" />
</p>

## Pré-requisitos

## Mobile

:warning: [Node](https://nodejs.org/en/download/)

:warning: [React Native](https://reactnative.dev/docs/environment-setup)

<p>Seguir os passos de configuração do ambiente</p>

## Backend

:warning: [Node](https://nodejs.org/en/download/)

## Frontend

:warning: [Node](https://nodejs.org/en/download/)

:warning: [ReactJS](https://pt-br.reactjs.org/docs/create-a-new-react-app.html#create-react-app)

## Banco de dados

Para poder salvar os dados no backend, precisa de um banco SQL instalado. Como se trata de apenas um trabalho acadêmico, recomenda-se instalar um servidor de código aberto, vamos recomendar o XAMPP. Ele possui versões para os principais sistemas operacionais (Windows, Linux e MacOS).

:warning: [XAMPP](https://www.apachefriends.org/pt_br/download.html)

Depois de instalado, abra o phpMyAdmin ou o terminal e crie o banco de dados. Pode dar o nome que preferir para o banco, só lembre de alterar depois no arquivo [api/mysql.js](https://github.com/gusbdev/FazenTECH/blob/master/api/mysql.js). Depois crie as seguintes tabelas:

```
create table usuario(
	id int primary key auto_increment,
    email varchar(200),
    nome varchar(200),
    senha varchar(200)
);

create table produto(
	id int primary key auto_increment,
    nome varchar(200),
    preco double,
    descricao varchar(2000),
    foto blob null
);
```

## Como rodar a aplicação :arrow_forward:

No terminal, clone o projeto:

```
git clone https://github.com/gusbdev/FazenTECH/
```

Depois de clonar o projeto, seguir os passos para cada parte do projeto:

### Mobile ([app](https://github.com/gusbdev/FazenTECH/tree/master/app))

Abrir o diretório app no terminal de alguma IDE ou simplesmente em um terminal do seu S.O e executar o comando:

```
npm install
```

ou

```
yarn install
```

Depois, execute o comando:

```
npx react-native run-android
```

Caso tenha configurado o ambiente corretamente, um celular será emulado no seu computador ou se configurou um dispositivo físico, a instalação do aplicativo será feita nele.

### Backend ([api](https://github.com/gusbdev/FazenTECH/tree/master/api))

Abrir o diretório api no terminal de alguma IDE ou simplesmente em um terminal do seu S.O e executar o comando:

```
npm install
```

Isso irá instalar as dependências usadas no projeto.

Depois, execute o comando:

```
npm start
```

Isso irá executar o server, que está configurado na porta 3333.

### Frontend ([web](https://github.com/gusbdev/FazenTECH/tree/master/api))

Abrir o diretório web no terminal de alguma IDE ou simplesmente em um terminal do seu S.O e executar o comando:

```
npm install
```

Isso irá instalar as dependências usadas no projeto.

Depois, execute o comando:

```
npm start
```

Isso irá executar a versão web no seu navegador padrão. Está configurado na porta 3000.

## Como rodar os testes

Coloque um passo a passo para executar os testes

```
$ npm test, rspec, etc
```

## Iniciando/Configurando banco de dados

Se for necessário configurar algo antes de iniciar o banco de dados insira os comandos a serem executados

## Linguagens, dependencias e libs utilizadas :books:

- [React Native](https://reactnative.dev/docs/getting-started)
- [Vector Icons](https://github.com/oblador/react-native-vector-icons)

...

Liste as tecnologias utilizadas no projeto que **não** forem reconhecidas pelo Github

## Resolvendo Problemas :exclamation:

Em [issues]() foram abertos alguns problemas gerados durante o desenvolvimento desse projeto e como foram resolvidos.

## Tarefas em aberto

:memo: Interface funcional

:memo: Cadastro de usuários

:memo: Catálogo de produtos em forma de lista, com a foto do produto, nome e preço, com um
elemento que possibilite escolher a quantidade

:memo: Tela para revisar a compra (produtos, quantidades, preço final...) com um botão para enviar
o pedido (Aqui, como se trata de um protótipo, todas as informações relevantes ao pedido devem
ser enviadas por e-mail, para simular o envio ao servidor)

## Desenvolvedores/Contribuintes :octocat:

[<img src="https://avatars2.githubusercontent.com/u/44094756?s=460&u=a2a2631e8eb8f5f5cdff75121eb422188a64bb85&v=4" width=115><br><sub>Gustavo Barbosa</sub>](https://github.com/gusbdev)

## Licença

The [MIT License]() (MIT)
