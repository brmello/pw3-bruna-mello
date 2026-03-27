🚀 Projeto Laravel - Guia de Inicialização

O Laravel é um framework PHP moderno que facilita o desenvolvimento de aplicações web de forma organizada e eficiente, utilizando o padrão MVC (Model-View-Controller).

💠 Pré-requisitos

Antes de começar, certifique-se de ter instalado:

PHP 8.1+ → Linguagem principal do Laravel
Composer → Gerenciador de dependências do PHP
Node.js + npm → Gerenciamento de pacotes frontend e build de assets
Banco de dados → MySQL, PostgreSQL ou SQLite
(Opcional) Laravel Installer → Para criação rápida de projetos
📚 Passo a Passo
🛠 Criar a aplicação Laravel
laravel new example-app

Cria um novo projeto Laravel completo com todas as dependências.

📂 Acessar a pasta do projeto
cd example-app
📦 Instalar dependências frontend
npm install && npm run build
npm install → Instala bibliotecas JS
npm run build → Compila os assets para produção
⚙️ Iniciar ambiente de desenvolvimento
composer run dev

Esse comando inicia:

Servidor local (http://localhost:8000)
Vite (hot reload do frontend)
Queue worker (tarefas em segundo plano)
🔧 Configuração do ambiente
Criar arquivo .env
cp .env.example .env
php artisan key:generate
🗄 Configurar banco de dados

Edite o arquivo .env:

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=exemplo
DB_USERNAME=root
DB_PASSWORD=secret
🧱 Rodar migrations
php artisan migrate

Cria as tabelas necessárias no banco de dados.

🧪 Testar aplicação

Acesse no navegador:

http://localhost:8000

Se aparecer a página padrão do Laravel, está tudo funcionando ✅

🧩 Criar um Controller (exemplo)
php artisan make:controller HelloController
🌐 Links úteis
📖 https://laravel.com/docs
🎓 https://laracasts.com
🐘 https://www.php.net/docs.php
✅ Resumo

Você:

Instalou as dependências
Criou o projeto
Configurou o ambiente
Preparou o banco de dados
Rodou a aplicação

Agora é só começar a desenvolver 🚀
