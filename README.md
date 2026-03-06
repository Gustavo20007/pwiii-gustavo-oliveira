# pwiii-gustavo-oliveira
Aula de programação de web III com o professor joão síles


//criar uma documentação sobre como criar uma aplicação laravel

Documentação: Criando uma Aplicação com Laravel
1. Introdução
O Laravel é um framework PHP utilizado para criar aplicações web modernas. Ele oferece ferramentas que facilitam o desenvolvimento, como roteamento, gerenciamento de banco de dados e sistema de templates.

A documentação oficial do Laravel apresenta um processo simples para iniciar um projeto, desde a instalação até a execução da aplicação.


2. Pré-requisitos
Antes de criar uma aplicação Laravel, é necessário instalar alguns softwares:
- PHP versão 8 ou superior
- Composer
- Node.js e NPM (para dependências front-end)
- Um banco de dados como MySQL ou SQLite

Essas ferramentas são necessárias para executar o framework e instalar suas dependências.


3. Instalando o Laravel
No terminal, execute o comando abaixo para instalar o instalador do Laravel:
composer global require laravel/installer


4. Criando uma Aplicação Laravel
Após instalar o Laravel, crie um novo projeto com o comando:
laravel new nome-do-projeto
O instalador poderá pedir algumas configurações iniciais, como banco de dados e ferramentas de testes. Após finalizar, o projeto será criado automaticamente.


5. Estrutura do Projeto
Quando o projeto é criado, o Laravel gera várias pastas importantes:

app – Contém controllers, models e a lógica do sistema
routes – Arquivos de rotas da aplicação
resources – Views e arquivos de interface
database – Migrações e configurações do banco de dados
config – Arquivos de configuração
public – Arquivos públicos acessados pelo navegador

Essa estrutura segue o padrão MVC (Model-View-Controller).


6. Executando a Aplicação
Para iniciar o servidor local, execute um dos comandos abaixo:
composer run dev
ou
php artisan serve
Depois disso, a aplicação poderá ser acessada pelo navegador no endereço:
http://localhost:8000


7. Criando a Primeira Rota
As rotas definem as URLs da aplicação. Elas ficam no arquivo routes/web.php.

Exemplo de rota simples:

Route::get('/', function () {
    return 'Minha primeira aplicação Laravel';
});


8. Configurando o Banco de Dados
O Laravel utiliza o arquivo .env para armazenar configurações do ambiente.

Exemplo de configuração:

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=

Após configurar, execute o comando:
php artisan migrate

Esse comando cria as tabelas necessárias no banco de dados.


9. Conclusão
O Laravel oferece uma estrutura completa para desenvolvimento web em PHP. Com poucos comandos é possível instalar o framework, criar um projeto, configurar o banco de dados e iniciar uma aplicação.
