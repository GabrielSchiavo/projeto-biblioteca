# Projeto Biblioteca - Trabalho Programação WEB III
<p align="left">
    <img src="https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen?style=for-the-badge"/>
    <img src="https://img.shields.io/github/license/GabrielSchiavo/projeto-biblioteca?color=blue&style=for-the-badge"/>
</p>

Este projeto visa controlar o cadastro dos livros e empréstimos de uma biblioteca.

* `Gênero:` (código, descrição) deverá ter uma tela para listar os gêneros, para cadastrar e botão para excluir.

* `Livros:` (código, cod_genero, titulo, descrição, imagem da capa) deverá ter uma tela para listar os livros, para cadastrar e botão para excluir

* `Pessoa:` (código, nome, endereço, telefone, e-mail) deverá ter uma tela para listar as pessoas, para cadastrar e botão para excluir

* `Retirada/Devolução de Livros:` (código, data_retirada, data_entrega, pessoa_retirada, livro_retirado)

## :hammer: Funcionalidades do projeto
- `Cadastro de livros:` cadastro dos livros com título, descrição e imagem da capa.
- `Cadastro de pessoa:` cadastro de pessoa com nome, endereço, telefone e e-mail.
- `Cadastro da retirada e devolução:` cadastro da data de retirada, data de entrega, pessoa que retirou o livro e o livro retirado.
- `Cadastro de gênero do livro:` cadastro de descrição do gênero do livro.

<br>
<img src="./public/img/screenshots/screenshot1_tela_inicial.jpg" alt="Screenshot tela inicial"/>

## :file_folder: Acesso ao projeto
Você pode [acessar o código-fonte do projeto](https://github.com/GabrielSchiavo/projeto-biblioteca) ou [baixá-lo](https://github.com/GabrielSchiavo/projeto-biblioteca/archive/refs/heads/main.zip).

## 	:hammer_and_wrench: Abrir e rodar o projeto
Após baixar o projeto, você pode abrir com o Visual Studio Code. Para o projeto funcionar você deve ter configurado em seu PC:

* PHP - Versão >=8.1.2
* Composer - Versão >=2.2.6
* Banco de Dados MySQL

`Configurando o projeto:`
1. Na pasta de instalação do PHP edite o arquivo "php.ini", neste arquivo descomente a linha que diz "extension=fileinfo" removendo o ";" da frente.
   
2. `Baixar e atualizar dependências`. Na raiz do projeto abra um terminal e execute:
   ```bash
    composer update
    ```
    ```bash
    composer install
    ```
    ```bash
    npm update
    ```
    ```bash
    npm install
    ```
    
3. Após configurar todas essas ferramentas, abra o arquivo .env, localizado na raiz do projeto e altere as configurações de "DB_CONNECTION" para as configurações do seu MySQL. Exclua a pasta "storage", localizada em /public. Depois abra um terminal na raiz do projeto e execute os seguintes comandos:
```bash
php artisan migrate
```
```bash
php artisan storage:link
```

1. Agora o projeto está pronto para ser iniciado. Para isso execute no terminal o seguinte comando:
```bash
php artisan serve
```

## :white_check_mark: Tecnologias utilizadas
* `Bootstrap - 5.1.3`
* `Composer - 2.2.6`
* `Laravel - 9.3.0`
* `MySQL Database`
* `PHP - 8.1.3`
* `UIkit - 3.13.7`
