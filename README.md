<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

# Projeto FreelanceHours

**FreelanceHours** é uma aplicação desenvolvida em PHP, Laravel e Livewire, onde freelancers podem enviar propostas de horas que podem contribuir em determinado projeto.

## Tecnologias

<p>
  <img alt="PHP version" src="https://img.shields.io/static/v1?label=php&message=8.2&color=18181B&labelColor=5354FD">
  <img alt="Laravel version" src="https://img.shields.io/static/v1?label=laravel&message=11.9&color=18181B&labelColor=5354FD">
  <img alt="Livewire version" src="https://img.shields.io/static/v1?label=livewire&message=2.x&color=18181B&labelColor=5354FD">
  <img alt="Tailwind CSS version" src="https://img.shields.io/static/v1?label=tailwindcss&message=3.x&color=18181B&labelColor=5354FD">
   <a href="https://wakatime.com/badge/user/30563c84-4568-4594-9bbe-b31f0effd26b/project/b93cc11c-d341-4309-8a1c-a8600855e13e">
    <img src="https://wakatime.com/badge/user/30563c84-4568-4594-9bbe-b31f0effd26b/project/b93cc11c-d341-4309-8a1c-a8600855e13e.svg" alt="wakatime">
  </a>
</p>

## Conhecimentos Técnicos

- **Arquitetura MVC**: Implementação de Model, View e Controller para estruturar o projeto de forma eficiente.
- **PHP**: Utilização dos fundamentos do PHP para o desenvolvimento da aplicação backend.
- **Laravel**: Framework utilizado para desenvolvimento rápido e com uma abordagem baseada em convenções.
- **Livewire**: Criação de interfaces dinâmicas e interativas sem a necessidade de JavaScript.
- **SQLite**: Banco de dados utilizado no desenvolvimento local, com migrations para gestão de estrutura de dados.
- **Migrations**: Uso de migrations para versionamento e gerenciamento do banco de dados.
- **Factories e Seeders**: Criação de dados falsos para popular o banco de dados e facilitar os testes da aplicação.
- **Validações**: Implementação de regras de validação no backend para garantir a integridade dos dados.

## Instalação do Projeto

Siga os passos abaixo para instalar e configurar o projeto **FreelanceHours** em sua máquina local:

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/anaclaraaraujo/freelance-hours.git
   cd freelance-hours
   ```

2. **Instale as dependências do PHP**:
   Execute o seguinte comando para instalar as dependências necessárias:
   ```bash
   composer install
   ```

3. **Instale as dependências do Node.js**:
   Depois de instalar as dependências do PHP, execute:
   ```bash
   npm install
   ```

4. **Crie o arquivo `.env`**:
   Se o arquivo `.env` não existir, crie-o com base no arquivo de exemplo:
   ```bash
   cp .env.example .env
   ```
   Em seguida, edite o arquivo `.env` para configurar as variáveis de ambiente, especialmente as configurações do banco de dados.

5. **Gere a chave do aplicativo**:
   Execute o seguinte comando para gerar a chave do aplicativo:
   ```bash
   php artisan key:generate
   ```

6. **Crie o banco de dados SQLite**:
   Certifique-se de que o arquivo `database.sqlite` exista no diretório `database`. Se não existir, crie-o:
   ```bash
   touch database/database.sqlite
   ```

7. **Execute as migrações**:
   Para criar as tabelas no banco de dados, execute:
   ```bash
   php artisan migrate
   ```

8. **(Opcional) Popular o banco de dados com dados de exemplo**:
   Se você quiser popular o banco de dados com dados de exemplo, execute:
   ```bash
   php artisan migrate:fresh --seed
   ```

9. **Compile os ativos**:
   Para compilar os ativos front-end, execute:
   ```bash
   npm run dev
   ```

10. **Inicie o servidor**:
    Finalmente, inicie o servidor embutido do Laravel:
    ```bash
    php artisan serve
    ```
O aplicativo estará disponível em [http://localhost:8000/](http://localhost:8000/).

## Licença

Este projeto está licenciado sob a [MIT license](https://opensource.org/licenses/MIT).
