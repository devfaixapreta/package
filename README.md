# Package
Exemplo como pacote

# Install package em um projeto
## Instalando com um arquivo composer.json
1. Crie um o arquivo `composer.json` na raiz do seu projeto.
2. Edite o arquivo acrescentando o endereço do repositório e a versão ou a branch
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
3. Execute o comando install na pasta do projeto
```
composer install
```

## Instalando com composer
Você pode instalar o pacote diretamente em um projeto adicionando a dependecia por linha de comando
```
composer require devfaixapreta/package
```
ou
```
composer require devfaixapreta/package "versao ou branch"
```