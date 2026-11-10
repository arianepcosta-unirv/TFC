# Societra

Sistema web para gerenciamento financeiro entre dois sócios.

## Sobre o projeto

O Societra é um projeto acadêmico desenvolvido para registrar e acompanhar operações financeiras entre dois sócios de uma empresa.

O sistema tem como objetivo organizar informações sobre aportes, reembolsos, retiradas e fechamentos financeiros, oferecendo maior transparência e rastreabilidade às operações.

O desenvolvimento segue o Documento de Especificação de Requisitos de Software (DERS) do projeto.

**Status:** Em desenvolvimento.

## Tecnologias

- PHP 8.5
- Laravel 13
- MySQL 8.4
- Bootstrap 5.3
- Composer
- Node.js e npm
- Vite
- PHPUnit 12
- Larastan 3
- Git e GitHub

## Requisitos para desenvolvimento

É necessário ter PHP, Composer, MySQL, Node.js, npm e Git instalados.

O projeto utiliza um banco MySQL chamado `societra` no ambiente de desenvolvimento local.

## Instalação local

Clone o repositório:

```bash
git clone https://github.com/arianepcosta-unirv/TFC.git
cd TFC/src
```

Instale as dependências PHP e JavaScript:

```bash
composer install
npm install
```

Crie o arquivo de configuração local a partir do modelo `.env.example` e configure as variáveis de conexão com o MySQL.

Gere a chave da aplicação:

```bash
php artisan key:generate
```

Compile os arquivos do frontend:

```bash
npm run build
```

Inicie o servidor de desenvolvimento:

```bash
php artisan serve
```

A aplicação poderá ser acessada em `http://127.0.0.1:8000`.

**Observação:** a estrutura de tabelas específica do Societra ainda será implementada nas próximas etapas do desenvolvimento.

## Testes e análise estática

Execute os testes automatizados:

```bash
php artisan test
```

Execute a análise estática:

```bash
php vendor/bin/phpstan analyse
```

## Organização do repositório

```
.
├── docs/          # Documentação do projeto
│   ├── Diagramas/ # Diagramas (casos de uso, sequência, classes, ER etc.)
│   └── Prototipos/# Protótipos das telas
└── src/           # Código-fonte da aplicação Laravel
```

Todos os comandos de instalação, testes e análise estática devem ser executados dentro da pasta `src/`.

As atividades são acompanhadas por meio das issues do GitHub.

## Segurança

O arquivo `.env` contém configurações locais e não deve ser enviado ao repositório.

Senhas e outras credenciais devem permanecer fora do controle de versões.