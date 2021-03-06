<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## Sobre o projeto

Esse projeto é um modelo padrão com exemplos para serem utilizados em projetos Larael.

Para utilizar esse pacote, você precisa ter os seguintes componentes/programas instalados na sua máquina:

- PHP >= 7.2
- Composer
- Gitbash (para quem estiver usando Windows)


## Instalação
### 1) Clone/Fork para a máquina local

Faça o clone/fork desse repositório para a sua máquina local. Utilize o comando:
 
 ```git clone https://github.com/matheusflauzino/modelo-laravel.git```
 
 Caso precisar fazer o Fork, utilize o botão *Fork* no topo da página desse repositório.
 
 ### 2) Atualizar as dependências com o Composer
 
 Após o download, faça a atualização das dependências utilizando o comando:
 
 ```composer install```
 
 caso não funcionar, use:
 
 ```composer update```
 
 ### 3) Crie o banco MySQL
 
 No **phpMyAdmin** (ou via terminal) crie um banco de dados chamado: *banco_unis*. 
 
 
 _obs.: caso esse banco exista, faça o drop (excluir) nele e crie novamente_
 
 
 ### 4) Configuração do .env
 
 Altere o arquivo .env na raiz do projeto (caso não existir, duplique o .env.example renomeando para .env)
 
 Altere as seguintes informações:
 ```
 DB_DATABASE=banco_unis
 DB_USERNAME=SEU_USUARIO_AQUI
 DB_PASSWORD=SUA_SENHA_AQUI
 ```
 
 Observe que tem que colocar seu usuário e senha do banco de dados local.
 
 ### 5) Rodando migrate e seed
 
 Para criar as tabelas do banco de dados, utilize o comando:
 
 ```php artisan migrate```
 
 Com esse comando será criado toda a estrutura da tabela.
 
 Para popular o nosso banco de dados com algumas informações, para que não precisemos fazer cadastro, utilize a seed (mais informações [aqui](https://laravel.com/docs/5.7/seeding))
 
 Para rodar as seed (popular o banco), rode o comando
 
 ```php artisan db:seed```

 
 
 