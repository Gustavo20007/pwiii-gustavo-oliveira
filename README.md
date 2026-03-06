# pwiii-gustavo-oliveira
Aula de programação de web III com o professor joão síles


//criar uma documentação sobre como criar uma aplicação laravel

Documentação: Criando uma Aplicação com Laravel
1. Introdução

O Laravel é um framework PHP utilizado para criar aplicações web modernas. Ele oferece ferramentas que facilitam o desenvolvimento, como roteamento, gerenciamento de banco de dados e sistema de templates.

A documentação oficial disponível no site Laravel Official Documentation apresenta um processo simples para iniciar um projeto, desde a instalação até a execução da aplicação.

2. Pré-requisitos

Antes de criar uma aplicação Laravel, é necessário instalar alguns softwares:

PHP versão 8 ou superior

Composer

Node.js e NPM (para dependências front-end)

Um banco de dados como MySQL ou SQLite

Essas ferramentas são necessárias para executar o framework e instalar suas dependências.

3. Instalando o Laravel

Após instalar o PHP e o Composer, o próximo passo é instalar o instalador do Laravel.

No terminal, execute:

composer global require laravel/installer

Esse comando instala o instalador oficial do Laravel no sistema.

4. Criando uma Aplicação Laravel

Depois de instalar o Laravel, é possível criar um novo projeto com o comando:

laravel new nome-do-projeto

O instalador irá perguntar algumas configurações iniciais, como:

framework de testes

banco de dados

instalação das dependências JavaScript

Após finalizar, o projeto será criado automaticamente com toda a estrutura necessária.

5. Estrutura do Projeto

Quando o projeto é criado, o Laravel gera várias pastas importantes.

Pasta	Função
app	Contém controllers, models e lógica do sistema
routes	Arquivos de rotas da aplicação
resources	Views e arquivos de interface
database	Migrações e configurações do banco
config	Arquivos de configuração
public	Arquivos públicos acessados pelo navegador

Essa estrutura ajuda a organizar o projeto seguindo o padrão MVC (Model-View-Controller).

6. Executando a Aplicação

Para iniciar o servidor local, execute:

composer run dev

Ou:

php artisan serve

Depois disso, a aplicação poderá ser acessada no navegador através do endereço:

http://localhost:8000

Se a instalação estiver correta, aparecerá a página inicial do Laravel.

7. Criando a Primeira Rota

As rotas definem as URLs da aplicação.

Elas ficam no arquivo:

routes/web.php

Exemplo de rota simples:

Route::get('/', function () {
    return "Minha primeira aplicação Laravel";
});

Quando o usuário acessar a página inicial, essa mensagem será exibida.

8. Configurando o Banco de Dados

O Laravel utiliza o arquivo .env para armazenar configurações do ambiente.

Exemplo de configuração para MySQL:

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=

Depois de configurar, execute:

php artisan migrate

Esse comando cria as tabelas necessárias no banco de dados.

9. Conclusão

O Laravel oferece uma estrutura completa para desenvolvimento web em PHP. Com poucos comandos é possível instalar o framework, criar um projeto, configurar o banco de dados e iniciar uma aplicação.

A documentação oficial disponível em Laravel Official Documentation fornece guias detalhados para aprofundar o desenvolvimento e explorar recursos avançados do framework.