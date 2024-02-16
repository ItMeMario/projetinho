Projeto Template Laravel com Docker
Este é um projeto de template simples para começar a desenvolver aplicativos web usando o framework Laravel com o ambiente Dockerizado. Este template inclui configurações básicas para iniciar seu projeto de forma rápida e fácil.

Dependências
Antes de começar, certifique-se de ter as seguintes dependências instaladas em sua máquina:

Docker: Instalação Docker
Docker Compose: Instalação Docker Compose
Certifique-se de que você tenha permissões adequadas para executar comandos Docker sem a necessidade de sudo.

Como usar
Clone este repositório para o seu ambiente local:

git clone https://github.com/ItMeMario/projeto-template-laravel-docker](https://github.com/ItMeMario/projetinho/).git
Navegue até o diretório do projeto: cd projeto-template-laravel-docker
Construa as imagens Docker e inicie os contêineres: docker-compose up -d --build

Este comando irá baixar as imagens necessárias, construir as imagens do Docker e iniciar os contêineres.

Acesse a aplicação Laravel:

Você pode acessar sua aplicação Laravel em http://localhost em seu navegador web.

Comandos Úteis do Docker Compose
docker-compose up -d: Inicia os contêineres em segundo plano.
docker-compose down: Para e remove os contêineres, redes e volumes.
docker-compose exec <service-name> <command>: Executa um comando em um serviço específico. Por exemplo, docker-compose exec app php artisan migrate.
Estrutura do Projeto
docker/: Contém os arquivos de configuração do Docker.
src/: Diretório raiz da aplicação Laravel.
