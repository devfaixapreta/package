# Package
Exemplo como pacote

# Install package em um projeto
## Utilizando um arquivo composer.json
* Crie um o arquivo `composer.json` na raiz do seu projeto.
* Edite o arquivo acrescentando o endereço do repositório e a versão ou a branch
```
  "repositories": [
        {
            "type": "git",
            "url": "https://github.com/devfaixapreta/package"
        }
    ],

    "require": {
        "devfaixapreta/package": "*"
    }
```
* Execute o comando install na pasta do projeto
```
composer install
```